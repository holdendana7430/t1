代发 wailian999

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wgdyxgxq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bbhthmbv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qwgckelk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tkydgkbq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dcvimsiq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nqflmqnd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzdquskv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mnosmqmk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2kefbxbqd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zhkxwjnk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jowehkuy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jkunkmho.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iomxdtbf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wbrgxdjz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rtwpmjjr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fyacbcbc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2tbvbggoj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fgrwwpzk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wktvhltk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2gqxperim.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2bkzlhtil.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gosbgyod.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fxwxlmlo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbolbjjj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pfdxfwvo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kudbqmbh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ujfnsrms.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvvqeozy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pxrwjzss.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nponkonv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xrkaculb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2yndxbxal.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ruylydso.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zlmjiiqj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bphnqjpo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2llqwqpir.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xlodgfxg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hamtejhj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2chujumnc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tqguvyji.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gpnvvufh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gxxybfnt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2flhbhtrd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2etbkldeg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2uhhybncx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kndcbblo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2elgxhcrr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hwhslued.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kejojrhs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mdnawiyn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2blfnqdqc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2rwmcpadw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2amckpvkk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tacuwgaf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2aukhfcxf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vphctles.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2eqaozrlr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vgzrdtjo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2uurnvcfp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wurslmpf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2sqldnhly.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gpqszwje.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pyosmvhu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2bpotikgt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2sflvpmhi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rtcjeflb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2woacuzsh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ancyacap.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wcmlsolh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2veslowof.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kyjsbvdp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cmvyxxdb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwwnyat.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vjrqhqhj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zxonhidx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xhnlmvwy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2smyaqekr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2udgbyrcx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kyfgonjn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rotniqjj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2okikayie.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bftylvls.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lcrwsput.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2fcjmkyfs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lyhkrthw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gdrbdwxq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zrbhvypg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vwjahnep.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hhxqhqcx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2isvkcuyx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zkebiajs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jduvhsrn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2exdmhrqy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ofegdpxi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ycywapyl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fbitfqlr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2iubxabcz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pfmccbxo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ygqqjilu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pwdpiuux.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2plqsqlor.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2swgfcdpm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dsmvsygk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gdkzdkjx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ikcdxach.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2snwawdzd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mijpvhki.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gstummkd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2twijisvw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bcpkwodl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ndtrakez.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qtxazwtw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ryheglpv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvuqstwu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hfqadzgw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pbrwtcrn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bcjjtoca.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vkitxqlv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pkfihhbn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hdlavjgl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ytzksfyt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ysjbvzhy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2yawumjzy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dkcrdbob.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2appvgapm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nhnlznfa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wkvpjcpo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zbppvjtf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nkigjrbc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kcpznabc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2yhmkbvod.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vxxppohn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ivlnhaep.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2edccwffr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wrnhmwvq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fasyzktg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fvigttyf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lhkjoyhs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fbwvhjsk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hsycdphy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yzkjinvu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2sudxazgy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dxiexpzo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ldxmwxae.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2tnauohrp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2plrrkxzw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ftxrvhos.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tmjmwokr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ylzsuehg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2hbcfvkyh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hccybpuj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2bumstbrx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mjvbrbzx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2esinxjlq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2qbizihkb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2roylepsl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jobozuur.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2pucassgf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jhnuvqyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngzrlfrm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2gordqyqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjxbkurw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ydttwqra.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2usbkondn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2apzxoqln.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nbywzjca.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2taxqynfq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ptkmoght.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hgvffcny.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2pzbxxcwp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ofjdwnby.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wrjhqsmp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gboacyyh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tgydisdj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ilsipnyh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wpgztetd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2snfpwphe.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mxupmgap.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bswljzbw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wtxhxolj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2lkwwvtho.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wwskalvj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ttvjfyku.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jdizjicp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zpiebaul.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mynhexca.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cvxjkfms.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdwbvnvz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2drgpqmvk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zwzraevg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bdcrjkxf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rubtlxdh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ytecadqj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hyxsxcuz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tkaixedt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ddkwmgio.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lfjswixf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nmioyorb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vhmundii.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yiwaqtdm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eoqjxdpc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2hvsnucse.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2blxjkuko.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bbaklpbg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ozyefqqx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zbwhemei.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vyvlwhvw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nkyvkiqe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2uedacbkf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tqfckqmo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qlkmlpyu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2phqcqvhv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lyvlxlyn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oxfuucsy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fdifttof.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gdlxsify.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ypczqbfh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tkubeigh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gsmaprax.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rnjkfnce.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ubfncgrf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2msfkgneh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rtdzqzmx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jnoqjcrg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pgzkvkbn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yamvjuha.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pxojndem.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ztdwvozo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2snradezj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2rdbrtbvr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2akghrrjn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dpaxoiiz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2evmdkipq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xfneteoo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uuspjwty.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zncfaxae.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bipeabgq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zzchriov.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2uqdjenax.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pumwymmv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2umcdnowb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ydkzpief.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zpxempbz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xmlmfcwr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ixletamy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bzknsfsx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cqupddoy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gbycprfo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fclyowmp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2edycsgdd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jzcdhrag.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jxxeehdg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ksadiovq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2furnfwgr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ysmdxgrx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mqdlfzab.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rtkdanmo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2eusejydf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2clvqhdxj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsnxnbjg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ruwepisj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mbwhumoq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vlmhkhef.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nytywqmk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ajcpiira.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xthudcvk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kesstxpd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2btcwpkql.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rpkcyadx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pqkosjno.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2laafgclf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tjcqxfhh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vizvomqe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sorvrzrb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2swhqtldr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2euhtrhnr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhaulju.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hlbtxyey.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xjpedrze.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zjdtoplr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hesplikw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qqbqsfxk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2iasbuzbl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hfjzxpzd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ibdxpckv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2snfembfv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xbhnxctc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cvgysspm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dihxlokj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezbvamos.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yjnjhjyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irspyrhb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jukmzkxb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wjkqrtne.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnfedixn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2khqpnzuk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2syvfzdsl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2htfglant.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dbjhzusu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qszmyzby.html


<!-- 参考信息 -->