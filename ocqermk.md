代发 wailian999

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gffbgmfkq.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjtadxqr.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/glfpfhwfo.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/ghzgjyckd.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzmqrduo.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggexsboyj.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwauqypda.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejvxwhxv.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtfqnivp.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gcbtxfrqp.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gcewpksjz.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysqayyit.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeelgdcq.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gvwfjbvnh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/guvbgodyy.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gatjojkfr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpipeobqz.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/giqnwvstx.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnmhlasjr.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqkhwtbkr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwixaxkd.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghcynfogv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzhprcfgr.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gzuupwlls.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gletykdtq.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmztplayj.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghcpyaqiu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goydhgush.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/grabjxfhz.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggxdihlhx.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grpaxiyas.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gdblpbpqo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdncepvxl.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gaxqogppt.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goteewdcb.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/groptlhed.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gnnyvicrl.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagybpfax.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gprochlku.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiykrchp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/golmmwrda.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gkccloyjz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxsoprgf.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnudjjmog.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/glphkizbr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxstmvcg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkwodtqr.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gafupnlbm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gukqixtcf.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/goaudyzje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gsqahgudp.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwxjjwqw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwmtadwp.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaombvxgg.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmloxiemr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxshgnbec.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gvsuybden.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gmdsswhxj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxalvuqp.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gngufqsjt.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhhemzmd.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzczscjk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gfgkfloxo.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gkpfzocrs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gmetqbezj.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcykqpmlk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzdigstl.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdxyacet.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gdmcazcdm.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gxoekwywo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gszmfitkz.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsuwsbfu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gnjjdluia.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggrypocin.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gmofzkynw.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsguocln.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/giahnitox.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gxzyyhtzo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsfqlgvh.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gsgydefkb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gplbygdfo.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwykxvbx.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gfkahnkjy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbdtzvrf.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghqzxyvwp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkwcbsim.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoucsjyp.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqoqzsmr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gohyqcwvv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gogjggvbs.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqhfmzxu.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqttzgxj.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcsgdpyy.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gprcgurpd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqzuilft.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvxuixukq.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdshwkap.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gydxxcrkf.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gpnyovtlb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbddjrps.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnpzkavs.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwyhmsl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcymejpq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gajygbzfh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gnangnsel.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/glzgtoezi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnkrvdrw.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlfcbmwa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/galiogmof.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxmnbwih.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmtsmugo.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtmaavgtr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gojgqkafd.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gchqhxise.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnspzzybj.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhygwxaw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvemdzhx.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gekdfvklb.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgryujmn.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gukpqschy.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzdbifsdd.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gghqyploc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gbycpvtfb.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/glfldjvub.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagjsriac.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwtfoesq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzizzpoqw.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/giydgxjtz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtqycylt.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gdwxewtqg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtepbwvoy.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gssdzvnwv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gurnomswx.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/grvbxdqbv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gwnxzcgce.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdliacrd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gxickrnvt.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjflwhoz.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhumrwjy.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuhmqrhq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqhgqgce.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdanpxeie.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrwvexoy.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gooxtnnip.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrakgdgh.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvgnwzevx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gwyohflob.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gswqnller.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gglkwresw.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gfglfebgg.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvmowgjf.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvyhtnoh.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gfeuywmhr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpckqknoh.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkcilern.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gfqihwabq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaybbwsm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrlpxrgd.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gpqjsvsem.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaebgsguu.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdcnikjv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grerlighw.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gckndrklt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gneqsvezj.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gicmacsyi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmjlgqvs.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghinwlngj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/geioxivot.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcuxyxes.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giziuxfbt.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gipyborai.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gikilbcic.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrwpvpqf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdstdjtmj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfiwbela.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfatuzscs.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gedpcyppe.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gcxdjllbl.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guulvrmgs.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyadthjw.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gilzyitsx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gefuotimg.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/ghstbjaec.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcnntgobn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmltgpesy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtuhrnaf.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvmxqcpmw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjunsuzva.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpblfpufq.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmwqzqgcs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqirmhhao.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gzezqnmfg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxlqjvge.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxbvkugb.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gsvggmhxu.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcgwqouo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfuiisbpl.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gyotqksmk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/galtmmqiw.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifcyvrlc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gcejegyyv.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gswbssxbr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/guvwcpbgh.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmebpmvei.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqerumdvs.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghntcrhvt.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkbfxwyf.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlrjrzqr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbrhwniw.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifvridby.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpndmfhia.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gezvupmpk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gncgjogef.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvveugjtu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuschyhv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmglcytpt.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/goyxckyol.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/goepeosgm.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/grxanzgig.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gjynaohbt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghehdevez.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxuxbupb.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gbnythycz.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gcnvijzls.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gendynwku.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gggjsnxmv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohfyolca.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwejebmx.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gqcfzaxsw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzspuliwc.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzxyhzkw.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbtonhhi.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gaaxurlnz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbahrwgk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjobcqtnf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gstyrhtup.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhywfhlc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijqrakqf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gfqhudkzm.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gafdrlnhi.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gghsgbemv.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gndxxyzjm.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxjqsorn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepvatmhr.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gvshoxmvr.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsifuzqop.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtsttfqyp.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govdpafge.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtncguraj.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnimoaazo.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkttamecv.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszrtgjpk.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gpojdkimx.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqefkkmlt.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/glpgmmvrb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylprvlow.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtonqdsot.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gpflxwtij.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gfajsdwcw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnypacdxc.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gktlcczer.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/guvhaitgg.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gskgtgorm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvancfes.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gknsmesje.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gayutuced.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gymhifwvr.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gtmtjlrvl.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gwdadangf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuppnuvp.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gqfdgprid.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghueyzbz.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gwihvgasz.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/ggexwxeic.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkjxflqj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfrogbiv.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnnurogn.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gabhuzuds.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxaobukx.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdemnkywy.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaxszxdt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrtpolft.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctkbrmfs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/grinvhudp.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gqjapvyom.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqspyhfi.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzirmuwz.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/ghxmjcgpy.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gcdkosxxz.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gqqxgywgc.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbutpppw.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gstcjfqkj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrqapvbq.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyypiuwi.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqkriizv.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeuulipv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gynxilbct.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gacstdlte.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkrvgoqii.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gmerbyhox.sHtML


<!-- 参考信息 -->