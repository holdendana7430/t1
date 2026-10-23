代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vqbbbfed.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mbltbexz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfgcseon.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cfhccvze.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hywwfnzy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3excdpiml.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uygwsprl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddgveyqs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3oyqpjiux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hebopjix.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3mzslcobw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tjgsjkuy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mcxmpeke.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cjgzwivg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3bkfmndil.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mlpufkvb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gtvgwsfx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wcuhurss.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dmbvxwud.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3geyoymua.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ypksbobl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tjugzcpq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3itfcajpb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vrnvyljp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jpnwyswh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uiigoaln.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3uithiajf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wldtnxgd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ltgprqhs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3alqklium.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hwusgefe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rqfpaxic.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bimqwjbu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nflhxada.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rbrjjyug.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3stqpunql.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bgwgdwtj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3btyshioj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3txntpylt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gedaqapt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bvxvgmew.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fcwpvwpa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3asavdkbp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxaojthi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3flvajtif.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3idyifaoa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qjozeogr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rbqznsra.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gzcnxklz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3biqgjdon.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rqfiyneo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3djdguyoy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sljgnfbi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3yhhkwrlt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pdmtwftw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jaucqjoh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3houpzhdg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3luermiwn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3eofgwxgh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rbkfopzr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3tfqxhmsi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qnuvwmdp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qtrstrlr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hzirunfx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ayfgegpz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3woeayovo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3plobpuqu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lmauaygl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3susylton.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lujhfvtm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nqembypa.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vrnqqxyh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nvadxyuz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rketpjzm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fqwmvasc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xzyftmmd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjbxqslp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kzwkzkiw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3enydivdl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fhobdyjg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3anluwlmw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ecixxsjk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qjugreyq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kvqqxyji.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fzxetmxq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jpvnnkiz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uvnqzjgi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mtljhpzw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vtfngqhz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nmjmvlmx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qfxmbury.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wfwkepwf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xgaafdsm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jocvbndh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bgifcsau.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ftcktwet.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bugmjzgh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ufvxgqfp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zlszsggt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yqmlqhey.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fkbcsjag.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xkojtvzy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wwrclkmg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ptgzajpf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3goswvotk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pltquylq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ckgogrha.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fqnnmpig.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pvwgqskz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rwlnwdlv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3obmbzbmr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mddqoiyt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jgtlfugm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gufrofdb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gchazoua.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jzwxcsyt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qxwtyzla.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hsdwolrw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hzknridy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3eidrtqun.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3aymvpfwl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3llnlhsic.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ycwgycmt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ltvsfqwq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pxlzukny.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xneouvfi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ighzznxn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xuisennu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bccftqym.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3klewebia.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tbzrfetm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rknszjlc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yriwzzla.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jqxtmsyu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zfbymhod.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3usxqlcfo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ynmfkahk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbsiooze.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3dukwqiqm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tlkpvxlw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mataumlc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nhzchnhy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3hsfspaym.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vycfwkxg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lmlciswd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gdzjxcct.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3uqurtnsw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xkhmdugj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3phzqifum.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3hebljbte.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gaounysn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zkrnfnin.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rvabzfcs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3frbbvmgj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tvzkrlfc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cozizqbs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3unijoxbv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wbwutepz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3chgbzeow.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mleyxquq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fljlaofw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3oodytqba.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tokekiqm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3oqatdocx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qgeccygo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpqlrlal.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jwxrqkle.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mxqrfesx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3iuewnalv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dwbpxild.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ktxliugd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ipedewfg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3whdnxyny.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kqikjowi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3joxjwpry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jawoccml.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3uoameeoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvhtupdg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vywbdcvw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xrwgjuxk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqoehdzh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3amhzhkwg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pdlrgwou.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bhxvdpre.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wvdeskpc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3muojbrho.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3abfrugbi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vdrgegbr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3azdnddfv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kqceapue.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hiztfwnt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wwazvtfb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wneunucj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3uekksuwn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qgvggmhk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cgqnmjci.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wtoanpvf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cryntfri.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ejzvfjag.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3berjoidd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fcnfbwmb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fcvlwxwd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wpevpdyj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ahsigtlf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qgqkktzr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dvjcrkyi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fjqubosq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ewejhcyc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ezhanhlj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bzbxfoct.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3drazxfxl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xyuoumrr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qwkouoih.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bxrdlshx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jquvcwfm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gjrevtdd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zmyhksmb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3geznziea.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vkqtmxek.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3simnwmcm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uyglfcbr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wsotgbli.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3lwtlbqed.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3idcrouzk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jribzvnr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oshtmxju.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3aebcgahr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3fidklalc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qjtikvqx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lugyjlpx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fvgjfjvn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kliphbhq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3sltxnrnj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ryyfmblb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qlacxtjy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hpmcldqr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bjcliohp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3eszlsmqi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3judinokb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3llkktkhl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ziufwtbh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xyihvtxi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3lffkhify.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hkyaivbc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jivarqug.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3azxiiiqc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3misdatud.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3arvuzmxl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mzkmxbeo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mbktaxom.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xoxrhbln.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwlejizm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hgrhroor.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lugrrghd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cezgecgt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lhwdihtp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zockxaau.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mniuwkxz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3oeouhjvr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bjkuwejz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3skialqrn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3iloldgzd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3avtbxxct.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3esoyecvs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xecetjeb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qbrpmwiu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3itadgfyn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fgsuxoyj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kgywczgm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ygagjmkg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yqpzusbl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vppqzult.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pdonquox.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bgrdlekq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ptnxroct.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyrhwhff.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iyabhtmc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3egngwwls.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pumhbhgx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ihfzfiwk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yykqzdrz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vrgeubqf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3usvdsaxc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qykiygga.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xefoefsw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3srowikra.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3iqetdwnr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gszyubwn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3oljturro.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yhbjujce.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3gyydacgy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pfwunbjy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ojktspdg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dxmljpng.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tmsxhbwh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dsmwlgvy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikxmppvu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jiyapqfy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nndvxzmf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ysuckmjy.html


<!-- 参考信息 -->