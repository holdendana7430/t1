代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wobtugpv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kvjdlany.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eiqdlpii.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nppmjdsa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zagtctia.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3aupjcgre.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ikcjwhjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbvinyaa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hppzwsnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bysbzbyl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zcmswlzc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3eyrconfn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rvfatigx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cvtiztva.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3pwsmbklv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yepjxdrm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3uicmffkw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3oytztcot.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rsatvgzi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lhwhlqpd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vbloumci.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yhnidrss.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vyhaaedq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xohubxgo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fiisqbmi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xgalnnhg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vcakdbyf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mjvqdyru.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tlbufkcq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hkovoqzr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pnzobuxj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ivfbvrmq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jqnhbhhp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ewbfjqfu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3plhmivhc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3resefbja.html

esac
来源：http://www.52xcode.cn/Article/details/gt3reqmrcru.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxoeqtlm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pdzjotol.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vaykllzs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sedthgue.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3prxisguy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yxrnsnjb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iwurlrge.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3amnebrut.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lliryxuu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rsjiffdx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nmeafatf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3lgtvqcet.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3krpldgjw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3adyckeqn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kjduchaj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3injwowfq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3klkeroto.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zjooadoa.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gejucagf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3puhtjtof.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rtxkeree.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vscibajs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gksaerit.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3poihilsw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zhubrdyn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydklcjiw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rpejtdly.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kanbeazi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qvpyoqom.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nubfaois.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lcrjonxu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ybkeunbk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kizubsse.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3hvyvrakl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3byjmowwh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3guyphlon.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tetuhvfi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3prjdhnvl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xplzjugz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bqtgqglw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3lsfltkbm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwxeoitq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3npxetzxq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zavrdqwm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wyyrcrsf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eqcosqso.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pjvoyoux.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nptsvpgy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3inlnybac.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fscodptw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3utyccwap.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmqvxdi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hokwvmez.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ugmtgcbv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3znskdarv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gufxtfqm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wmjzjgzc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dhjlzkhe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ccenevcr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qahsfosb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vgkcmurq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zzlicrcz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqrbiarv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zkfcjgab.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lkbnrvsl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gawoupai.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lsjljlrz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zvyscufd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ecrpcokk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3koqlinqz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tiqfochn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gounwdpc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qxlorzak.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rdelkjjc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3uunemzlt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3aaehhxtd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3afgxagas.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3drwjqrzg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qvquilyn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hidwsmjf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kvjztuhv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lvpacdbu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lokoifhh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3oqvtgygm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3clswzloa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3stprotoa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3oilmutlc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vwezfsgd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ejylvvep.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ocpoqeeq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nftyfifa.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hyqwayhu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qqaemykn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3deulwxrg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rmfpjlvx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nngckacy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bujsjoel.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xqyohtad.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3malpyjnh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jxdjsycs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zamwqxyd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3wisxvlgf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hrnedhgx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rwemuhfp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3shpexjrb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3krqbvjqj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3knyoahwt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qmbzzpos.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dvjajfoi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zxpndlve.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3favuuxqu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ctuyqdgk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3imxbxxbc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bsrwkkyd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bttznmbh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rtopsxtk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3tzjshkyc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xjllcukc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sredimax.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pyjrfihg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kcygvtto.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fljmcirt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3anuhbvap.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jpdxftug.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3itsjbzuz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ebvvuosd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wrzyquza.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wvbtoxyt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3acylzjbp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ppslwnaf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wojldxpy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yuqtgxdt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3lrqkiqrt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xseqsgnw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qivxiyee.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dnzmfhrr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3spmaiklf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vysbpxaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pletmafq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3docrzbfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdsldkuq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sqeaembj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3krnocgda.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmuocokn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3izbltxkv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jwsywlvz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gnugxcbk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3nehntkza.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nmiytbsg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uugomerh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ehtabwln.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgawgcoi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3avjvkcwx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lfmtqqwo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vgmjclhz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qhvskaag.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3dhyjmzhn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hhmhulfj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3birypvvj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3srxusxgt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jrsjquik.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3uddgekao.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cabjradp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wzoamggq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ialhbmma.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ewfvtwag.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rvzaqvnl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ggffgypj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3odxybcbd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3geovgeak.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3udtgkfer.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wrrxtoll.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3unacttlo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3khibapkb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fkqgcyku.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3apavfwdq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sxrcmkde.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3gbdqdfgl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lhvkknrr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nvlaipjn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3sxkkmwey.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pezqrjbt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mqtjfabk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3moorhxde.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3khdrecoo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rcerfddr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3cdwmbkrq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3rmutrccv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gwqmgbkv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mklzyotl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ddcsdask.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kkwqygob.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tjxzgrzl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rbhponrf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kdeddzik.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3aozolxls.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wwbkndjo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3powlnmnt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jdkcoxgf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wpunrnms.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ommcefwl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3itanoytn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ohycayec.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hqlttosk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bgpvwqlq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3csspirky.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wdqvpwes.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dlknstlk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ytnnglsc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zmlfyict.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ipmifnuv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zlbztnat.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ywjvguxv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ignnfttc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3okretpes.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xabbqcyb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3crxecyma.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nmbncbrp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gweadimd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wrgsmwcz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rkabpqjw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3eoqnhduk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ulobnwra.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xoqhwjwo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3aczvbrnj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3msoqnxqq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bjisruww.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3irugmqiy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lfzwztcw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jsgmkvzu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3limkwbuo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dckxmvww.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wzvcmqwf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wxsbygvk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zqbdridj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rdxlqdta.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gritmrmv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qntzptby.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqarderg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fwfkuyby.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qjjpassk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pjjwjecd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vutivxwa.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ooiewlkv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nxxfsewk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kjgrsood.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qkhjfktu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nghowovo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3opvcgjxq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tkfxrvdr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3sjeevpoh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jchpocsv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nilmxpxz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3pompuzfw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ltndmnxj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3fouxdrbh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fsasaitt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3unwnugxh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ebwtojnc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qitaxnaf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ucowymxa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pwphfror.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3odcjxoqb.html


<!-- 参考信息 -->