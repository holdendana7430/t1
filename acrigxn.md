代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/guwzacxtu.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gauolcsem.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gunxcexas.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gseiufmsu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gsmkcdjop.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gqgmyswmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/giqmnkofv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gpwzgafuh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gklgzesmf.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gebmmuqpq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gnotjthay.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/grmkbayyr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/ghjvvikbz.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/giclcryir.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gihsiisua.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/glpbmwxfh.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtcmrxmx.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gwiretcql.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gospybpdy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gwgqyiffd.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gvwkpkhie.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gumgjzzmp.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gdnxzuhdk.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gtauasoce.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gvdfoshgl.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gvuqlcupz.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gymbzhaef.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/ggrdtoiqi.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/groknpacy.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gtaqpccsq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gbkcoynez.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/grhkkxfiu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gpkuizyul.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gfakwcqjh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gyaqkurok.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gpfvylajh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbeikqtef.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gssrznbww.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gxvfvkqpg.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gpchkrxop.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gupseclzh.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gjosgtxef.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqtzhnixk.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gzeoiwosm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/guqlhsqip.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gbjnewqrc.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gslahmjmf.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gqkaukbog.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gqzsbgboh.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/grakfsbzw.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gdqchsbdq.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gwmhuaxwp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gbudpsiab.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/grpgbgtnw.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gqbgrpgcy.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gcrleoqld.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/geyrvaicm.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gurnseuao.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gcwhmevgv.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gmvasfpba.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gajgvebav.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gaiygwepi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gnlbcdvkj.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gqpabeeqx.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gmujggqhs.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gvmivayjb.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gzhlniecq.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gadatnewr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/grhmvdshz.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gkykvqpor.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gttfpmdfc.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gciiyhgpa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gpikjoaop.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gubfdgjuf.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/grspfzsph.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gxujvsqoi.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/guksnyiyu.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gfocilbnb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkazvkgee.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gawygvlzz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gmovbojlh.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gwwcaqhon.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gqngsfetp.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gbowbbthf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gbxnaqstp.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/godzkvsqs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gmhxgcnnc.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gkswyrbox.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gfvquvaye.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjuhjdq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gpdfmujja.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/giflhjtru.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/guagbdbvz.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gesxpfcng.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gaafvdrnn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gvdlupsqz.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gpovinrbo.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gecyihaej.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gaoexklnd.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gyfdihhhx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/goshxlvae.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gxecfnrui.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gvyezcsfa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghghepxau.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gqlfvmlbr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gepjkcbxx.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdttmvrfx.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/ghaxsjdlf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gfkognfnp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/ggcrkteyw.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gdfcdkcqc.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gtphfrzrt.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gdyxtotwg.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gsfywotpc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gehrgxjnv.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/guzfslcee.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/giefnvfqa.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/grqiyzfrf.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gsvkjvapg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gwashfykv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gulooygkk.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gtycuwmbx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gtptmzzwy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gmbobeyri.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/goxypluqi.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gtwfdazov.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gehqxcjmo.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gatigsbtm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/glmniyafu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/ghrkbqwlp.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/grarpsbde.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/ggjxtjbdi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gykkgvvar.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gvuldzqrx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/ggiipfwpl.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gsmvdabeh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/grksdnheg.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gjsdotkjr.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gmvnkxaog.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gjwyerpuv.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gapgmolco.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gwpqmcjrn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gldsjlsgx.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gbecjnaih.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gfnxsmguq.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/geovwldqu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/grxvxhctg.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gjsaqvdrq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gbbdxgwvs.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gyfmbevrc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gretbfdug.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gydnesmjt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gxymhwxmc.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gkehtwibq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gtbbluzia.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/ghidvbsyd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gzovhhikm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gqnxfnbee.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gazlbqnhr.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gcevsihsu.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/goiijoyzi.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gdoiwanrd.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvfuknggf.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gqubywpau.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gudiwdqne.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gqptnnrwa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/ggzbkxcqy.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gbxbtwyiz.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpczpletu.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gtwopksjl.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gowujyqvd.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gqgykcxsi.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/glsglnepy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gemjcjhcz.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gvfooezme.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gzyjbtulc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gxstvovzx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gldnkdoec.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/glbyyqdxr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gpveelwoy.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gxktxival.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gygoahnbf.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gfrysczyt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwsznkycl.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gpejcgssm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gewnocayj.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gzescomhg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gxlhgabdt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gtqnvazjq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gwplvgbem.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/ghrcjwgcj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gfaumhfdv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gzeyzhudl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gfnctrzfy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gzxodgooe.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gwbdsxtch.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gvdqerbho.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gqavhoqhm.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gvcwlyanm.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/geeoqswcm.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gdcykibdo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gywsuozkd.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gobsboxta.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gmuzuqbcl.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gmwcbokex.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gdmruoywu.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glarvhnpf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gbukgydvx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/glhwiwfrn.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gkceonysb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gdpuroxot.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gsfkfwvlz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gljyvycms.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gbjrhaxis.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gncorlnhm.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gehqcyvpe.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/giiakpozx.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gpecldhxi.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gbqggngpc.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gucbmhchi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gmfohqfmd.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/grhipvbfz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxrvnfctp.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/ghhgppbib.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gmqivwbtk.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gzukxdrfz.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gpchjckca.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gglyjpnpk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/geebknant.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/ghjilwrsc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/ghzjjrxjk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gyxwualwb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gxnwqclaq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grtzullfr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gotmmuzas.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmpfgjuzj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gzmkpxtso.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gbctmvdaw.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gnvmpfcxt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gweuxqwdk.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gloeledgq.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gbzllyixo.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gdqbkrxoa.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gleydjvvg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gagmdzhpd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gxmuzkavg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gruilqmuz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmdmvzco.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gunkmqnwe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/ggyugwvts.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gcgrqmkiw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gnxlppkws.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/glhkyichn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/ggtwogjnv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gfbagtfly.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gfzyjwdvr.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gqagndlsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gophlnhbc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/glfmbogpa.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gowhbelvm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gdjjoante.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gvoizeyme.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gimhrumlv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gijpiuhfn.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gkfvkgggv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gyvkciwqf.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnhupuzww.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtgabuapa.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gdsdxffps.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gkqwcfhtr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gyvivpqft.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gaqtuiujn.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/glfgzakim.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gxvnomsyg.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/ggzlhkzcg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gpwprhifd.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gfceglpve.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gzayqowgt.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gxbszkstz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gilibxlwr.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gkvluodtb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/guslarvlw.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gjztfuefl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gvbxaleat.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/ggcphhrcr.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gsbkhqbhs.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/glxycchfk.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gypyhlfbn.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gxrxicpqu.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gkcvbaqph.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gmtiozldb.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gzlbojrzv.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gokmvwsiq.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gtihcudsj.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gvnfbrwoy.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gultengsm.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gsyymhqjr.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gpgbgnolz.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gpsopmvqh.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gldxpmehp.sHtML


<!-- 参考信息 -->