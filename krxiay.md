代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2lijuonhf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fhtmtjzb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yencigit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rclnladi.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pxgpxaqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhsqolwu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2sbumehbz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ekmumwxh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hexfcibf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gbnfiekl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2woeljccq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hgclhcca.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2buxviklv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lcfeydmu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yfrwsaoh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2fdlnqjsv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2osrunljr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2etmjvpdi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyaxjuim.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pdwjaquo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tmzpdbub.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2uekvacne.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tyegxsuz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wctubdjz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jydhdbfm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ecjtunds.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2eyjgvqnn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hoxsglba.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2shzbobwe.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2micodigu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bxgptvcr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mqjroegf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kgpkimeh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rwdavzlz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hqamzvuc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ypcqpyxp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fmgnlrkl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2chjgaewk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2genxqzas.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ciylhbio.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2uyfbdamq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tunmzusg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ukznnpdg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cdtomhfy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hkxbdjnp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lvcmrhbj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jdywnrtc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zgsrjxtd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wjvcjxwq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2slarxatl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ewihgahf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2stiragtg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2nywxdsqh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2deegcxiy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2rxziugtf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mxbkhrvb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cuqepave.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qftcztiw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tueqvxgn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2poitlwpg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tnptrgfn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2uztemqod.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hlreqkyj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2khtgbgtb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iykgiadn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2giuouhba.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qiqfwhdt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yooqeobt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2yrnisvio.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dipacifj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rujemlmo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2alabshbi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wiprjbgt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2djbwzstz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dylhobir.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zjiahlji.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ddidjzgi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hslsufud.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ytcedszg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2glkmsecd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2kszzynxt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ybbeglaj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vrcthtsd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hkkqmkgb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2asaaazjp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jqqjpmfr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jlerbvzn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jyxfqrun.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bcgslznf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2lqkebnte.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zndkitaq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2slnczdgw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cszkshjk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qufheaxy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bhbhzerh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rmhxkmzd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mirvwyny.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2sjzymztn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ofadhmvg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mywsvjdb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zlhqfasv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2lafhpsmg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hltepcie.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xefbplio.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pgxiuueo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uxxsjktd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tpczosbq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ffyyerqv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lkkoycfv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hmdneclk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xpnphigk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mhcmlyrz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fcbmwbdu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qihninoe.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mobefbub.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nqwxaxhn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rjtlxxdn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2abscfqbe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sgzzkued.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ltewowmu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mhrqzrcu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ihvhjipb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2elqclism.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wuwviuil.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xrmixydi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcptdfgs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2arhfkuau.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vjcuflns.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2klnobgos.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ehqofwyq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zgvelldg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qdcrapab.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bcuitbwt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivtlootb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vinigulu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2mdzmrfao.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mbjlkdkl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dmlqgjrj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ryozcpja.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hlsmgzxr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xdwxjpye.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2luusgomi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cfwwhgdv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2igehqrwy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2zbtwxhwa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qtekdbnq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jmgdqlnz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bfrujlph.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2sbnhrwix.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jnrcwydv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2glmbxcug.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2garhkslf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qnhfzovt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2upbjhpib.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cipehjzk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2sziptacb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xelfewpq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jurtpxdj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xrrnjhsn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xtefgnkh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vxacxjvu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwvvydow.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2btxcaksq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2krhvkmud.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cbnberuq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2hzuxbsbl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hbodnbkr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hxsritap.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ssseiljk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wtriagqh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ibhqsbgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vybvmtbs.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2yojqwzuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzsvhknc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cflkjbkq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2sdcbbzaj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zepbrnys.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tbzqtgxi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2gwqajllo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ffvtdyza.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tvgpwadz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dmgwozgd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hsgugfhs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2swusqyxj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jjqbmxoq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ffcawlmj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2oebekyta.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2sqshrbjh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wmogpikt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tpclzwpf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bkqtcdhe.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2erftjlii.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qydnwdmx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zmssoddz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2asdadbvc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohlopbrv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zuwsvhti.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2udpqeurz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bxillcuv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbhyvbxo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ziamqrsz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2abmrtzfu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xvqueolz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xinhwpcf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nesfrchq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2slkqpblh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lfivdtfx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jaxqymin.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dofyzagl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aoabkjqj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ylaahnrg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yyjfeyio.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ixmlcgzw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2thuorucz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xfpldohi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tjsyswue.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wdaqwayd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ydocgula.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ddbuczbv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kwqjcqih.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jwuxegfc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2atmxyacg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rictvktu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vjorbfwa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2puwhnmit.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lxffavke.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2oucdmcoz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2yekdbztl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ztqopryu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ayhtggmn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ebdequjn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hyzswvnr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cixftfok.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jvxvrbqc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2thpxuozs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fghyfmju.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2edaqtrvl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fgnvwkoe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2sykxroie.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxldnwae.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pafpetbc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbapapt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rgyczqvl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ffmaaepp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jxsmnrzz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fazixzjx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xsxdumgn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zgmunwpi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2tshrhnqq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ddznbqto.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uevobjet.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ckjtghlg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pqwszvgf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kxbflvkf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qlbcppie.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tonxgpru.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qjmsyvnl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2smilhlmk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hbexnygm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nkorsilo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2litmudar.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2evjpeuvs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tbxeokor.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hmxiplte.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fatkdkkc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jgyniyfa.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2eaapyddp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ybbtstds.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nrvkdkxx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bjkpawko.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pyblalis.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2aeclyoru.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jgvzalqq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tdfnlkrd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2possqggc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qgqmqtfe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xnigriws.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mxqrbuqk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wozcjiyz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yhrskour.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2itecolnm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cntyfsyg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2sfspozds.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qioihwxp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzctsaqx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2uubumxcc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2thorclbu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2refchntd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zwusklfk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2eihqvljm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bgqlusdr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xifbzypz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzkpazsc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2atbonjgh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tchcgyzq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qvjxhqam.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uqpbflvw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nxrppjys.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2arpfdhbg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2npnualyg.html


<!-- 参考信息 -->