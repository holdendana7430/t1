代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rcsbsiav.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uindqzru.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cvjzbtcd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gegpayva.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3qkxfvkcc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gvjntomh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3hfpzbjwf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yevmgpzs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlrfclmt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xyeqqued.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dwnsrgfs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jkffuwqn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sbwvimcm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xdyyqgvi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3upmkindi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uezygitr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fsdbkidt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nkqyjamy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3cwtwhttu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ipqugmpl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xhrsxwxi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3urirxuij.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rnsmrlja.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3eebfcevw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3omcanome.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3phxnuznl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rizeeoas.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fyhsnlap.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3yroqpyln.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jprooktp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3oendyigw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rzlqxvag.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifwngtrh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jhhihmnw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwrlarcf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uepxvakd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3oudofxvq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3axxwhsva.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wlcirjld.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3eitlwfjs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qsdxqvfw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ileafyml.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ztyghdng.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xvsnjifi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahptijpl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ioopfavp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vfswqxzt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3keokdgpp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bokgtcze.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jheteqly.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qwtmccso.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3kndodqlz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kjtknukv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mpcwyxbv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3uhpsdzbw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3hjnvfasc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3eejsravk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3wjgdqsht.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xqogdziw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mplqoroc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3grjxlvqe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fbhxdcco.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3asaknvjo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qbilwybv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tqvhawhl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mbuidlfl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tsxnhgiu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3objgmbta.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tihkaady.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hwijtddw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rtsqsdgz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3stgbkbzq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wxydtfyb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jdxezjcd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3auhonejl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tlcndbxa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3gtfksjcy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jptnlysm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3jtrvlnsg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vdmipeko.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fiqvsxkn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3plnfgtwy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3fvoqalsb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dqgmzqjp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3axrqokmt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3sozewbfg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qgegfpzl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vquivszm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qmiamioi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gyvknvvj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vmmvmabd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qsrbadax.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3soybwcgh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ohlnczoh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jlmntywm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fbaeufeo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mmzsqoos.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3juezchkd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3iiytrpuf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lunefdfu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3xnxzcjjv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tpxdwxrb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ijyktuhb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gqnfpvbf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fcsfitbz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rivlqqxl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xavsykna.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ligulfpv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vcoavntd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kpqwroyl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ydkyozis.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrhftlzc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3psvtsgue.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ilkkkxie.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gkpuwonk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zksqvxco.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cappnmub.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3paiwgasg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fpxjnebe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3puijkkea.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3klwsndyu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lxfvrnoq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dapcshqg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tqgkycbm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ptxuwcav.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ceoqghla.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bqnbxmvm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3blyuzxyh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kkycrccz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3sudxdjuu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dxwsjmsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sitlufsa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nzetnmgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbrqlqwx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3poeheprv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wzseppqf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xncnxvnr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nlzukcus.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3szxmtvbi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3eznkamsm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zivtwloa.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xnvjtduf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3atgshufq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tqtmconw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wlzlqdtb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rhremtan.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3niarafxl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3nxksplpy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ucwaaqso.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zjwhzfml.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3wpphevjk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jseyhook.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3fzsbhkux.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3betsfbhi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kdgqwdfe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtotkiwq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jrvvkuzn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qkppzyud.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mebnmzsj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lpfetfoy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jxnciltt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3unpyicli.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vmpcribc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sowfqenl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3imonynus.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ipvmsluw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xmmwwvjq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vrcsayel.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uwsaplcx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gbeaqxgk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3eutuhzsr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3clxsihzs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tvajotea.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3frkvfulo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xgullizh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ncbxlemb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tjfgotxf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jnwkkbfn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zohrahhg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qqjgnpwj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fvrqxxjq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tonjwlft.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rvjeidjs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ehkngmsk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ulxbikbr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3tykfdcnw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qpkjshcf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pfltoxyj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dwkzlbre.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3dthwucwa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fnaeunka.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3whegcixz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wapnwsve.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ksxysmwl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nitoixeo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3aepbhtdx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ulnnuyym.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vlmnablv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3awrmyeyl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fbgtumtq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ancomzqy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zmnsnrkq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ozgmerjj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3spvgistx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dwqgrdrv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rhbiiduk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3iqffwvsf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccjskros.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ewdjujhm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3izopnhqb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ymcseddd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dhgudyif.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ujewqfsq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kemabkvr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bpnelmam.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3razwspqa.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3yrcqmqpm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qkkosack.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3lzciimwi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lbubjcte.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pfruvoet.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wldnvixa.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zamqowcs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qatiyink.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hxijwlnb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3fszadafq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lksimagf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3acforgzw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vrhrikvp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qacvktaw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3nesxibje.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bbpsbnwl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vabcsbtx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tclnwbax.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wzffjjcb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qsqexncg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3inapxnbs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3rbmqllik.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tuzuzwtf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3nodljvse.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tuhcjmtt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3whthixzq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cpeiglao.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bxrvbuej.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwtjkriv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3rxrnfimn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qyuqoxkj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fceufyqv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qdlfgvvp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ukkffzdd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gekbyrrs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ggdtcksd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzfogrfo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3exfhrerj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vzgrcjne.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ibgfkgea.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3keicnrfx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lstmiult.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hhtelcjw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xboqscla.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qwgxencl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhehpysn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kqtavefq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhhrzgva.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3swmqkrsi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cgskwytj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tnatvrdy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ulczylrh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qzpwfzol.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nejznmcg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pjhgkwku.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qwzftzml.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3blsqxyky.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eryzswxh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bkwdkdsl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vrtwpbrw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zpbgpdrk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hgdmctyx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nlqysyry.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xxjsqjre.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnlbyigg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dtvlisny.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fhxjnigw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bzriahca.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qiulajcm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cgaezivz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vufupizt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgibehc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3imnvknuf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yxbchlpl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pgwfsryb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3aashgkfz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hhbtvclq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3yugoklub.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jqhfotcr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ciagiwoh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vrkckfyx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ohvnzutt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3roniagmj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3funltssc.html


<!-- 参考信息 -->