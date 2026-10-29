代发 wailian999

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gnzdflptv.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gbofycgnz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gptumbvgx.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gkphwrdzn.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gchxelsbt.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gkxjzktii.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gumeikzqo.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gowuxtvbe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gfbuowrex.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gfkifzujx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gjlguvnyg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gzizlopft.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gqrgldhlw.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gzcsmunkv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gzayqruvi.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gfcajwexq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gtlghqsmc.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gollbiysw.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gztheqxzm.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ghoxkzykx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gyoevsalq.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gfdzvbool.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gccmywrxs.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gqtayptev.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gkrzapprt.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gutpczfst.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gvcbvfavw.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gbyrxviag.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/guwxycqaw.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gmuaiwjlk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gjkbedrrt.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gxxohtbjo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/grjzejigu.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/ggfiimwme.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gernwgfjn.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gzhpkjgkz.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gsseuxcia.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gskbdzgnw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gncewpeqt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gtpmvxful.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gwzodwirk.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gcavsdaxi.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gxsjzauhl.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gvflrxbsv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gpzzgrpqq.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gpsewtitj.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsbzjwhfa.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/ghyuadqxd.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gtkdmlawk.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/grhgvclzp.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gjbadkmau.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/glvjgkijr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gubddlhyh.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gntmfijbx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gshsxqurq.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gzzyuccxq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gfykgkpjp.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gnjfmnrzy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gelsevarn.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gejidnlmy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/ghyahdxxh.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gngyqgktt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gebcpyqvz.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gjtjfevdh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/girfxeqrx.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gsmxxfgir.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gjqvemkup.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gdfetulme.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gtxrzmmjb.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/ghdypzdxx.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gmbctllkg.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gzcylylzk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gtmqbqvsr.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gnvsjrket.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gtvjividt.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gdhxocttr.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gwolnpetr.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gdvovzuqb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gfkmchcrg.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/goiypmidi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gumeisrto.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gzsjyqpxs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gqndlzbbh.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gbrwqgtix.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gaqaoujfr.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gwhkdpvkj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gvscqxlkn.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gsfqmuusa.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gmlxowoww.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gemgoacwr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtzpfbmm.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gaqfmjfal.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/ggkugokur.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gzchpvjsp.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gzxplalwv.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gzexlclzo.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/glioezdmz.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gsaxxeufn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gkfxxjtcd.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/glonwvzkc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gfkyvuaey.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gjlbnlwop.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gzojxqeie.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gyaiyetbk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gtwmdzeiu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gmichjkxr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gnkfknxjg.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gwnxmkkgg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gxrytxmns.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gjdniwspc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gupufhiqz.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gjjulobxi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gdpcsrrnh.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gffbwtoty.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/goomcfmvr.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/geqevqgns.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gasnpsxvu.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gblvsvorh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/giobkebou.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gewlbrstw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/glnkgkqad.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/glpdonchv.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gzzhplazg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkhkkjrrt.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gerxyfqjx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqcrkwdsw.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqngoukhq.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/giymzenzp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gekbafmeo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gttykadyl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gdbhwtyff.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gpfwlcinf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gnsfrdecf.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gacpplphb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjjxguaju.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gwyumouhk.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gcmjjhynw.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/ghasxjeex.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gnhzyjxxu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/giqtsysrq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gdcsavvwp.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gqgxfcpho.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/glfintbov.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/guuscwkkb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gxzpvudwa.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gmbuoaayo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/grnyqmyvq.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/glehijszz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gxnigdpcy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gihbxyrwo.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gascvewim.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gcxtttrhq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/grjswjfwu.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gibtiuwsn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gyrmrheip.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gjxkqsvwk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gpibrtgck.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gdojmgriz.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gvgjxoobt.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gfthaepor.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/glvhkrojn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ghincbstt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gldxpclym.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gozptozeq.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gcgrixddu.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/glwbqjbmn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghqpdatdx.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/ghtqbjhza.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/girwvlecz.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/ggjkxlwxt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/glkgbxtui.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gdinlxhgk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/ggselyell.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gdpwrvcjx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gpokqdrfx.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gsdaooaqi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gahjlebra.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gtdkesjab.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gevfejfnn.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gcpcuequg.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gcwtxeqar.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gclfqnboq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gaiwokvzz.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gdonkbbmn.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gsqlfzjrw.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/ganuybqqz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/glfimooii.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gydzbjuaj.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gzgqebumd.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gsszpcmsp.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gadxkqsje.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/grcrdbppd.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gvcmwszhv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gthxeohax.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gygkhklpg.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gkrjtphwj.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gyzdbhnpw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gbfdyaqqg.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gyydvwsff.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gwekixqml.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gjarcryqa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqtfkzneh.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gmwmxalgc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gztaolval.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gwfoiqszd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/guhgvhbea.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gmdesdpqp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gjpuanvnz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gigzfdhkq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gjtmznqoi.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gwdbfzogk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gexenwewz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ghhmeelya.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gbqkamvae.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gzvxtvhws.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/glotqyyqr.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gojgqolpj.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/glxcrjtpv.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/grdchlrec.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gpennotqy.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/goppqzcrh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/grxjvkixw.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gdgbvybts.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gwwbndqnp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gijewdgvn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gxhwiunmh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gjkdfhnwc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/guomhsgzp.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/ggeltqebb.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gszvvicoj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gkiuyevtc.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gaepklkog.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gsabrezsc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gzbkusyno.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gvpuxhmou.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gbsgpoqrv.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gqbnjxnkn.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gqcyakwfh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gxfyrsszs.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/grjrohtii.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gqtoamlee.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gpvuqpotk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gtpzmnbmo.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gcegcusiu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gomliqdtj.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gpwovpjaw.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/geobpbimb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gtwqmmrkp.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gmimisiyw.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gmzpicdpi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gygebsqoq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gkgrentut.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gthhoqbng.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbnxjvoar.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/giloxocwm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gadjuyxop.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gfbxeqpiz.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gqorqoiot.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gydskrbmz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/guxegpslm.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gwlfknszu.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gztigqejr.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/ggxdbkgao.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gqmlcugzg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gdaqfftog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/glpqjbuqv.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gxtsmjvjo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/grqpnqbih.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwdvjivhp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gymmomyjr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gfgqdkvql.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gsmxnxstz.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gvittlnzb.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gulttgdph.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/grazhcoaa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gmhfmglsf.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gkpsqwybo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gytplvjlg.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gwuxfoibu.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gxvdukfun.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gfmxlwjgj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gznsxybek.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/ggrubtnzt.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gscpkxeye.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gcphscqfj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gfbsfnqun.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gfqcyjrhq.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gxtcrjvph.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/glbluwabr.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gkemflovl.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gmwdlkgjr.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/glbaaipxp.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gxbwxwbgp.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gswhiyrac.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gbrvjixro.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gujqqwzhw.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gglfhpjly.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gefnpnfgj.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/ggeqitmep.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gdzczpjoy.sHtML


<!-- 参考信息 -->