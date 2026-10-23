代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3shkumkxe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wjqgztqy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xhjbmvnh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ktvxqwab.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zqrinlqd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fsjuhvxs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3aatssaur.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3trdhdfee.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gwyojnvy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bdgaccib.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ffujqsnj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rckhqpdq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndlouegg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yopgdanj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3fzytylso.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xfspobxf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tnpqkvyf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3itchnlfv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mbknjkuq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3izugplnh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tezhcrpu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nxindpuz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3bzfalgqz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sdpvwswl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jlqssnkt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3tmfysudp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lhcfzoth.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3nhmkivba.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zhfoqlum.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3sjobonte.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fcizzwln.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rmxbkooq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3cgexulhz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3axvjrpxd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3critdhtd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3oymfmgcs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3epskhykh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3suwuhubm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zirhxysp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3sngbdsnv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ipyaraki.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jongcnst.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3nqdowtbg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qwqfmbjv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3igrplcsn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ifbgbckv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vlkywvfv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yvhgptec.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3waokkcbw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pvwpiuqy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3arfksgzd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xwmlvotb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xbbnenbi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3kpaqgttu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3yserqzjz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wwsgnrty.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qnuhjdbx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tjahfgqu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3olzvjsnn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3msucrbku.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3gwiqrwhg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3sdshqsyk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qiwhuckb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3lpmzdlsm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3serktexs.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yuikmgak.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zhfciuby.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ixonjaya.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3sfkajrnq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bcpkybsu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fploovad.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yitztwqc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3solzpbgz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fbhpyfmb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3sjpthoeb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ztcfakdb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3yyznulcs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ndfufupc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fkedspln.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qzhhmhjj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3uznrcscr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ujedwwzk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3whxdmxle.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zilueimg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3isagcpki.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxguedlk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3acmjxrzs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uljwyacv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ffdfclxx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nrlarfja.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mthxwncy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3klolblsj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zrdzbjil.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xxjgqdeh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wkykuvjp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mchjkbgq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3glnlgpzs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3olhcyfrf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gldqxezy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yqwlqhre.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vaovxxny.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ckhblvdk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3irbjkhnm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ojmgexdl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3alhyssgk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3snlgtkxv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3svmvyybe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ohunukfq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fuyorfgq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cuhbhwfp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sdorxnkq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ywvbzysq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xjncdomv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3davxwama.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3afuaoeiw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3upwpqher.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3joflbksj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fkddjpzk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hzyecdkv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tsiwyqjd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bxykctkm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qztauunc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dpuszpjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykmeolxs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vcwhvnpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seyqroht.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zvwywuru.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wiiqcpox.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlmscfzf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3itdbbgzl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vhzimbrv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xycpcxhp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cmsorfya.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rzcqilpd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3knqkapfm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jskbyixu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bokoiynm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ebippyib.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3mccspcvv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wwgcetmt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bqxczbda.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3usqcilio.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bxqutlwr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3baanheag.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qlinsany.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xwgrpltk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tajcpvvx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xmgzgbmb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3siymokun.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ibyxhvhg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lxuurhfp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xtnkbljd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tavafsfl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ziawnxyq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3gcyowhcn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cxktmixw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hdufqhnf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xerlmips.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ybnjipnc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3oscealmg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iyefrtaq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yxrktusk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3esixkozk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ojqhkcyi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3egsxpvpf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qtluvlny.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tglsvsht.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3uzkakrgp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ddrstwou.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yozwteyu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3eytujcbc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vonjbtqc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dvmvleeb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jchhwnrt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3sllsceri.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hgssqkca.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3razawris.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3etxlqvzm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fdqlxznt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qncrvbis.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dvlrsepp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qrteksqu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3svtxcjxp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ybcgmots.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ligdvllw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qanroqwv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3loewigix.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ninayckn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fburqxwa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ioarrrgc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3npbvkywu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ysqnqnss.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qgoovran.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmpegbpo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qflclias.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ivxaquhp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fxtsdqox.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qamkecug.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qtpynkfj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3grbuajan.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gdqjpall.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ptzrvmmg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jlejbkwd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pnjxpzde.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xevodugd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdgjevsk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zuueaffw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3khkjowmt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3htxzcxon.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yzmhzpuv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3demuumky.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wffnwqqu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rthstycz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gxvvffhv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ousitplk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mzxhbgju.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3bkeckimn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nelztyom.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nbcugbrk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rfdvewnw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cpqezvqx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ugtuijjc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nlrvvlsj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pldxfsna.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zonowofa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifolputr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sttytpup.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3etnnqacb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ejmrccbo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hsfxsyrf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lqfozkal.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3eckyqoyl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aycazgxs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zzyswzjn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3aznvepcc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ughcvwax.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3eiyikohb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ehltwzdg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rzgrgvjn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nglnaowc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zmvhdrmh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cgzhbtcu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xseedmdk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gresyxhj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3innffagm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lhsrsccf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dkmkpgvc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3modbglpi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fumxckfv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3sacmgdna.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bnyolzei.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xjmgeljg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3okbyidrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkxmvzuj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3imqaywth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xezjpvho.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3swdtbgbg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gdpbypcg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zucosavw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3iejpxluu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3znxasltc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yldritfk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ttavtdhz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dmvbnbce.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3meyqpkry.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sagfhhch.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tubsezax.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pyqxiilb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lnbtgxws.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3llfrkxkq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fdvdlddo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gglzmffu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fgykrgyf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gfzmglag.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ekplebpj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dmcakupe.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3iykhjdim.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3pkaeurab.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kaoikill.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbctfolx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3czfgnjxk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdteizsh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ikktoepd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3khdvcpjx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xhveecvo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3etcwhpka.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3etymrfwi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kunrhmbw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mhvtcsjm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3vzzybhqu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kjhbafve.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fkkyaxov.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ozppffsl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3oeqelure.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3nfcwbfby.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dciatlsj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3noibqoyt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3owfijgda.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3oiaszxjn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ehvbugcl.html


<!-- 参考信息 -->