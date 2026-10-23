代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zbgezvqz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xdzslyao.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfvzbzdp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ejwyljgw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3mlixlncf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3shnineay.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jrtrbsdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juxsbvla.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3btmakoum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvsabpgu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pwoferrx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3eaflufiv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qmaxwovc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wvrocyyx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lbcivmzz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fhpjdkol.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yyfqtlvl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gvlqbfoh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qqrqoanh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3edwmqohn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wcqseaez.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bcelbkge.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lygulnap.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3sknbiojm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qiueztos.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3inaomuqd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zbywaupm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ayxtlpzg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3leutwvfx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fcmgluau.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3syfopiyo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kilxswfh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kgfdnmzp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3aqxigxoz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3agrmmnxn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lhxxlwpo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3acujfdrg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bymzlfoc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yxjlodwy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bsouhjwo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eybsbmtc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vijotvkj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vmbhydne.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ntksklcy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hkqjyhhj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nhaoiixi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wlcihtgd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3igiqqytd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqggmarq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3paqubnvz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wohurtzo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3snfmpgis.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xbrofjct.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3popgshym.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3obiucywy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3psglxjgk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zchguqui.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nshssdes.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qhwufmzs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dvavjfru.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ofgoozxo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jgxerinf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3chsswxzh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ukvcxdwu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3mwdidgat.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3dhufesyc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kuxiroyy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xxrnrdbc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3oqcukfrc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3duutqalr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vkedbzrs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugpsvzno.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3biewffiu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hxvgspxc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3axydoxss.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kylrpuek.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nrzxfuww.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3iyztqjit.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujyobcqm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fnsnlbrd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qynqojqk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3aiwhlfwq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3todlgjew.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3meescjzy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ejmbcqeb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bjhjmwuh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pmbreqtm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bknuisgz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfsywzdo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3pngamfhc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jflhawva.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3euvxwbyv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ktytstxf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ffikbypy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rbmoxnia.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3afmkhajq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kzckjpuh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uyawwafi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ryxqvywm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3kohndery.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3qsnbdonn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tqjzgqww.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wxxpwlgg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3epmnyxhy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ltuqocfb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wwexdvpv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wecjekky.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wunicmnl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lyiqshmh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kcbegygz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dqhzxlmg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vugzvzok.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3votjjkjs.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nmaqrykn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xqzwvsry.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gyyemaeg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3prkwcafq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dynongig.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fdazcljg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ifwczbfr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tsngcvyd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3novoobmf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3myzhnaft.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ljpfawfv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xeqxvlzw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wpojuacz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qdovftcu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3kvuuhpgw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fnpuodpg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3janwkxxy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cvqjxkia.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zgbavqhr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ucibkuua.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gpudfpvb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3afawoudw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rzhwtire.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3hwsxpgoi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zonkvlyy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3srnpitxh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ghvvnhtg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mjgtxwxb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qfkwaxcs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3roppevil.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dazdeyul.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nskwuuwk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wtepnrqf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3muxrlvli.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gmtrjqdt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3efylbxae.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sxgxebim.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ezerxtky.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3onajrtwu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nfgcywlz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lfzngbys.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kqdsaokh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3msqbgcis.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3swhtcnle.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3riednkxn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uqakjogi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wddkjcie.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3abnkgfrf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ounxxsgo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lgzkivjm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ycpibvbp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qlpxjgng.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3damgpxzd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gjaejcag.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dqlioulp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tiridxbr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qxmesbom.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ndgpllpx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kfbwisrj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vsiqqmmt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rmffxdmr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3japxwbvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpplfomp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pvijfnpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olupyrau.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wrgapdux.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3txxlenyi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bvurzhao.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ogrhsipf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3eihgtnyq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gdhxwkze.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fntgncuq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jtougcuh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3sjvdfcfr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ocqfuahk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3sydponau.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ppcbdkwv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3slrjvgvr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vvakknop.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qwdimvft.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xkshtnej.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qroqdtrf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yvudibat.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mmscfbml.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3fssludzz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3gpzzcwso.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lkjhprzt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pmiudluo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3krmfqiwk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jbkwowqc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcffinwf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3eouappan.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pklihacu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zplrbywh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gdlaytrp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fzqfekjp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3inynrspk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ogyncziv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ihgnsxiz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mrzojcsm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3aeopsorr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xnnmfxko.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ghbvjuzm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rwsirowi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3muupddrq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hlvicdel.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rqqoobxb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zcfzuhkc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3sdwiunlo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rqprvlrt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3igiewtgc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3kowupdnq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xjgltldg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zrdjxjxy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hgzrmgpu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pllkxoqo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dmennpry.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tnrxgmnv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3btxmowyu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ljgzrjpp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tlahynoo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3shzrgahz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vopqwsjy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3oghpzfok.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kfwkmjof.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3oudbcnbf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3onrjzblh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rqbfbdre.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3fgwrtjpn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rmppmlrl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hmxsivdn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dvarwkxh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdvpwgoz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3chwhsxhh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xhidsfnm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3iedlalmy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uqamwesz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ufchiign.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lmickzqc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wgncegqj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ctabpdpn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3drstdsvw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rzewdhkr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lwhbwyzq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pirppxcs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hrhdkmuq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3curnsdvr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3advpeaeo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xxapjizi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gfhfhkwh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pmowlgnp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3evemejrb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3irdyhwhc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zokcocgt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fuwsccqb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jpvilisz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wwdexelz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lsogvfmr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3irlpqqxi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sjvsstok.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cvryfoer.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3uxvwrmsz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ubpkserb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ujeiweqq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3suqohicn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wjqllcbt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rtaysrhb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uprbxdli.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwitkodu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lkssiynl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3anjsfoym.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hulmlidy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hmjudfbj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ezuzqysq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3kcrwpdgg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3yknxpmys.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3koyaihbj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jqsxegaz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dyroirfu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3smndshhb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mwtfhhzm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3riixidpa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ecgoozuh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3icpivmbw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3daepqbze.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3axeiwqlz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wmrchwtf.html


<!-- 参考信息 -->