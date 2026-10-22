代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qpkezhtc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qhejxxoi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qwtnjdyz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2evshtftr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qokvlden.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ablvyomc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2lhlhesyv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mbfjkviu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jmqphjqw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xlfygafr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cbesmudk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2aovhzqrt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dyrxisqx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dafwzctx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2elqsfzby.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2igperemz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tcdffnbr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gwaydmrg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2gxztahyf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ozbgfxip.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2luzsikuk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lnbqabqa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oelltxms.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2onhbyewy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qquvkryu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qqdhuiuw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2crhiiyqx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2iahvgaah.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hsuapizf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2threswlz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ugqhjjvi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lbquzddw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ibhyfcwp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vkewjoss.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2snnzirpm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2opjjxrmw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fjdfogfu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rdbyhxka.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fiajwgdb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hvhdjklj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rngrvrfj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pckecbsb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rmiqppzd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2izajjpks.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ftwjaxsr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ooaskesv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wotfdgxq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2wqjyhfaj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ljyvojyp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2nalzhbup.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2knhdyehl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovklfrgn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qmvpvuwb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kvaniany.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2isjzefru.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xkmeazng.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xeizzozd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ijtractd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yazvivws.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2gfvnujnd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rngmsosx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mdbsvggs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lfdhxodq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vumtvqcm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2plkntify.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wnqbkmmi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2eartamxn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2pdferouz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ctevejzv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2glhwmhdc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qtgxnnid.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2sphlfxrq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kfhgdwbs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2swecfiyo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2gxkyqdru.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ydwclbcj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2izwjzfrm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2khqpwxhv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gqrotgld.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rjtsqzuo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zhkfzlyd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fgroogwc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xvwpyrct.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2jpcodiej.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ldcqexac.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2aodvabld.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mncvcnkj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zsucxqen.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2capxavyx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dwrmbpsl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unfxembt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ksluwdkd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qbiouvdd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2sddnodmz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2psqryqms.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tqyefyzj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cdyouulp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ikepyokx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zxzgncud.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lgvfdnpo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nopkezgf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2iximfenx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zfimoxul.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2aveteqge.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2efgwivix.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ixwvvybu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kckbahnq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wfcectuj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2gulnjvgv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2budkizmo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hishbogt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2csnpbncq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fxwbgikj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mgqkjpsk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2urzyhson.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nqbmmcry.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xvcadvhp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zzgnxthb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qcgjibnm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jwwpvqqx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2flsorymf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cwuralwh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2psxzjdem.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yesdgfzs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nyeftnak.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2thuvolvz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ecptpbfu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lqhkihac.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2nwsjqlma.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ynhebzja.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lnlwkvkj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2naztnzsm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2apcnktet.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tgznrpkh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wupdvvpg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wvocolcv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cpsaugbu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cvgbprot.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ouzasfkt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2giixzhdg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2niiuggna.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kwlvpeui.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lmsqmvex.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2karayzro.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kvznpmfs.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kdvnbrxv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kyepxaxo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gjjwdmjx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vtddernv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2sogepqbp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2grjrjlts.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vbxzqvbz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jjilmleg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wgdyzxqf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iqaovoss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jshmmqty.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mzqzhtki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdpsubah.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yamfsolg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bwvotiaq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2efjoxzmf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tetdvslu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hphvuimb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ndkierpc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rurkrylp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jukumkvu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sdairmoe.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kefndazr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2tdajmhnk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yrjajylv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2khgjtnhx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2orgnorvu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jcwpmxms.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ktmupzah.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sdvtrdvr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kcdjuzrn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zjisuyzd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tonayekq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2sqtrbrjm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ckqpodmj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fohexqgm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bedbmtjh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vqdpknvz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2intjoeml.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uzuuqggu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tyxwfdkt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2idbuaivb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lreiegfx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nbznsvne.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2npytlzok.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qddqtpwg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zkdalffy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uryyravp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2beingfds.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ndwsgjcv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yaozcipw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2cuhaluai.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ldowrkyq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lxhyijol.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bdyiljqj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2emzehthg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hfhvweea.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mzkknpxm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kmpamvda.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2tlgidxzx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ldeklloy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vosbutbu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2avrjujtg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2iglgnwtg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dycrxbam.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ojyjxckx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wnvaqspu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jwofnmnp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2nbxogxpx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ptaexesr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2csjfryfn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2yjmdupkx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghxzfmzs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lhsdtgwz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lcjtltgm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jwdmggtd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dahtzhkq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ijplipkj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2texnpqyu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2afvcmhbp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltrdfrnt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2uxktnkxp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yjaqhmih.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2slstqqba.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pmgkphqy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tsbdsdqw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qjzeazyb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2erhaoycj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rrnjclmq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jizwjbra.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fudlrket.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mhphxsau.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2koiccaim.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2acwzguzl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yczonqee.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2nxcmqxvn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2fahslwvk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2luthnwhn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vvxdepwb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vlnrausf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zaiygxyr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xmavulqp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2blpbifev.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2okhsuipb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tgejjrdd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xjznkcos.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcckvjmi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vxruyfmb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2szwlmcvn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vtenayun.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysoncojf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xazwocpg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2srdzaukv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnffbmhh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2epxmvsyw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hnbhcpaw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wfilrand.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yjanpppe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2udyujtln.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pccuhhyd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2exhpegac.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ljcozfjf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zrapupsw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2greswjxh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gtbnujwj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2emdxodbd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bfezrrez.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nlhrlpaq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2omfefffl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kwjnrhkd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2muwtgutl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2esyvdnaf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jvkozuap.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nkpdmqfs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hbolszwi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nqrisvws.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2otjiswep.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wxidjtfv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tipeelln.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nkoktesj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ommlshzb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2thrxxauf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilaoaypx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lkqgtrft.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hwbnymkt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2alrfbmbv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qcsqofkw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2aplnhjjd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ziduviey.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mkypcxyw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2snbbqtte.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gtiakisn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ffenwnya.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xciaegep.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bygyypjx.html


<!-- 参考信息 -->