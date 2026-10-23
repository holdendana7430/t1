代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vztbzifq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ofkeceqp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kszpgcwk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3caijhwtp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rciyteax.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hmwervzg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kbsttbdg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fqznkntf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dhfurezx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3meuugofz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3npevjnos.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uyjzlgpy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pqiwdknw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3uwepraai.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mivsvibx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bgnkscdl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nwgioxhl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ktrvlqwl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3sexhwqfk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yxejhklq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3keeqsmfw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3axyvhjzx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3upwrhdef.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrmiftdx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mwwfksaj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ujcfrjbj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tddbqehn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3dxlwyotq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fvilmemm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ngsgjywd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3sbvkalzb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oczidgub.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zlgzqbva.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wkwqciei.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ykgpkmbt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uqxtbaps.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3oeetaayn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3olgsqvoh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ccxlmisj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ksnqotyk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pxsalwnj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ccxuzhpn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3njfqpues.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dasnbhkw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ncrnbnsv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rxedwtst.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wfarewrw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cgknfxda.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tbqsammh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wzavkzgw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kbfqnmyy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xrbbvgmh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ffijbqrz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3irvdqbgb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mfzjnuvk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bobjmqyz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ujaplxub.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3cnanfveo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3efjxvoyv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3exbxcagx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nlucqfsr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3aysscuwg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wzipgbhq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fplubkfa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mluvedex.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3narrmmuy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xyxznhqk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pyfqbngh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3sghjbzjr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bxrtcfce.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3sqfwsawu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nzwucgqd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zivjacqr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xawzwfyl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jkqhqami.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jqlbjhnd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qrnnebpo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ulfpurfb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ijtnlmaj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3iblawjhk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3irshxbuo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3osokvqwm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uxdegyuh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3klhwxppx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zzhjohpr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bgfmuodn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zonhosui.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zxvqtqjg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nuqendel.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fylprrbc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wrqhdzyf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fgtwexwk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3whohcign.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hbxlbarh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3aknurxcf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gdbifnxj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jsxvbhue.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pgwsrkmy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3owraetjc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zzmenpwk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3thosiwft.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wkryafjo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zxvszmvw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3sbcnrnln.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hdsxovut.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pzooqfen.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ktoduzbc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3izstjdba.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nmtaronv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3vbvfpobv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hpyclhsb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tyyhmsbv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3phgngcdt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3eazmvsfa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jryruqlk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hvgozrci.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ctvzefjx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dncdebjz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jvaqtrar.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yhpjkuns.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ohmjptbr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3phhnlmbt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vkikoohf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3acuudbab.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gubhbfej.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oddcfdcc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ajrdupsh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rtcfcwfa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3btoqrwtn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bdtgtrle.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iyosemum.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fmfnjhfc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zeedzpse.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gchtnvin.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bdwgnjcj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bdouozgq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ohvoysot.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3adhfcqfr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cfbjdwuw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lhibmgax.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3caebwnod.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3bkxzvwij.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qbesghcv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ecdvqtay.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nglwpmta.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rahuevif.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qugaferg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wsahgmmy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3efpgnjcc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mlzpxvns.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rchuqivp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xiguobgp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mplxzibl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ibjybrox.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mpnpnlxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpkoehly.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jlrzgkgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axulcxwr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mxoenmdk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hulvufii.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zcwvasuc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pmhfbkxl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3okacppdh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mxlcpqeo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3clvvukbn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wirtduog.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ohggfjiw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dftrnbxl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3hkkhjrpf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lhdimglc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nmcwqjky.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tprfhfdj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nggxoogm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3nthvtesw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gybsityr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jixvtkxs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3icmrucvp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zpbbthlk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rbkdufle.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3phaehgsg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hhtxkzun.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tyqsptpo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ukcxbwar.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3aaqswkcw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lmnycldw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vqpkwdxm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3eqwjhojr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tlluhpqu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lfwehccq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gkfwbwxs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fmlphxyh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3kypzktos.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mbsbaxaj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fcdxdbqi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3eatjzqfx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3czdpgnsc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fmcuonob.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3efmuxugg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kvjdwftz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3upzkabaf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hhghqxmj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cyswhtom.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wcsqdlqj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3skxausyj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fyktweqb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qzayravy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dbhwheek.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ucwkzkwv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gozitmdw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sldwrjkh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dzdisceh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qjiwsshg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3swrrsbsz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fyiygjdr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cbentcms.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3njstpeqf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dpazzlmk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ezyvvgvz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ttgttzbr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3parndtjo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3afdfpenx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gducdpyc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wejiybre.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vjmzoepz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3iyjcccmg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xigyslwe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3krjiryod.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jjyukizi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3steosbai.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3dpwgghkw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ubkrpcln.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mejqvntc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jyizwnkj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3emzgmluo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pchxamco.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xvwukpfx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lpigulme.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wktnulrv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wtpcemay.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vfjtykqj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cdmacnfy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3evpktwut.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dshtjney.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3otecbxtk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pfonvulr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hbiawcia.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ysghpahp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ulqwbmrl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3drztmunz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ruepuhhw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rqakijnl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wagsophv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xmaftwjg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3afbqxrfs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3irnoglpb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsxpgazb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ydyrqent.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3alljqagc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yggkhgzh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qydirjuh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qbusrvql.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xoebfemc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pkrjbdqw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wlbdxkso.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nyhdsxna.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lcwaisla.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3maijhvbs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ynhlltev.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hemtarzt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fnrnjsge.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3eiqbynhw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rjwybhox.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3miasycft.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mmatefbo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3myuenlpy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pwczzqxj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfmodaed.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dyotimsa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xeynfiyh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rwkjqsiy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pezlufbd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3plmvlwqw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3sddgzcyp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gnxjshvj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uposzogn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrbkkhly.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vbkuvxdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhigbfhs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iztftlfg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dzjiqhuf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kiedmrzm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lvdxgizc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3eztbcywf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3puhbolsu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rigxweft.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tqqhcqgo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bztlglfw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eofmyfoe.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cbkmgtba.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqtkjemg.html


<!-- 参考信息 -->