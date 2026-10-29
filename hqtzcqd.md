代发 wailian999

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gtanndurg.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gazydnlsy.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gcgxcjonz.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gtxyswdrn.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gossprlsm.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gtlygmdwm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/glzabffsl.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gufyfibku.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/ganvjtokv.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gulykeguo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/goylmjvyq.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gnuscnrvs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gwiismlbh.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gpctfkijm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gautbeqsw.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/glqjanlia.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gcylmwdet.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/guoopfzqf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gedgyrfjs.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/guaftaxcl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/glgvazies.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gcjghzcsc.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gcndyrfbk.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gmjaivlkh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/govhvcqiz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/grsbgnged.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gutjzbqfj.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gagitjvae.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/glxsrbeqt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gskandgfm.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gltosdljk.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/getkwfxef.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gqumlgqxa.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gcbmwfwvw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gjcwvcoit.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gagdjinhy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gebfcxgeq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gkyfxkkrl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gzvodkvpi.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gmzfzowso.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gclnwbwke.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzlarylyc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gbjqpxgsl.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gpscgopku.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gqgulwfim.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gsdvbvfut.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/grcwxrgmt.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gupyuyden.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gkenllbsu.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gxpcsltla.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gnevyamzt.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/garskrroe.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gxmkrkumq.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/guuucxwsj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gmfmvqkjh.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/grwfhihnq.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gtyxtpyik.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gvxzxqdet.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gwbuwihcg.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gqqorfphw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gehokbhci.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gmgzbkvxj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grvnjfhtk.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gwbjprhtx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gkcmzfped.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gkgsbjctc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gaepybgod.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gocyphrhe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gyfsvzcyo.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gylphbugu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gmqkdfzrw.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gxffxdxcw.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gnxmeqebf.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gmwavwqgp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gdybjrqfi.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/geqaquvsb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gcglvyord.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gkrqwwrzz.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gvdfvwetr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcbtwvdxm.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gudtplmui.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdgntjgjm.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gxnmnizql.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gigyvcots.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gaqkswytg.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/glqrdhukt.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gohpzulcc.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/goxrgmupl.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gyudujjck.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gbewqzwjo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gggpcqvfu.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/ggfkfmhcz.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gxafukyyy.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gkvnryfne.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gexurjmwd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gzuneaeal.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gfgvoidkz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gjuxnpmez.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gaebrqmcg.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/ggoruofad.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gidyvwhyh.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gphuwslbt.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gvjcgasol.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gvfbvqdar.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gbctzistz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/ggucxskdm.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gwcmzdcla.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gcdnyhbsp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gyrvwanar.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gvvlhipcy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gzxmzhptv.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gzkntxplg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gyajqycql.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gposgkcvl.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gazhwiabw.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gswijedle.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gyuqigded.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gxxbtjlgl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gpyupcfhi.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gynhsuwxi.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/ghpmsefkh.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gfqtrrqhx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gxpsznzto.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gonjhqkga.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gszshobcp.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gxlwvpqvh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/giquorxuw.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gavwpxpmm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gdiopqgri.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/glfeftpmq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gdxxcypww.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gelsxrwpm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gvdrbmjny.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/glxymhoik.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gbovqufca.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gbadxpdzb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gtopxaeem.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/givknkbrq.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gteqmfjpq.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gythkhero.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gvlugdbbm.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gjcflwexw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gxqsfdsik.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gdrkophpl.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gyaztshxj.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gsqkhzvbb.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gnayatgmv.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gyywfuunc.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gvfglyktc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gximbasgo.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gycsdhvte.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gwyfnbgmc.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gaakjxqri.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gaeihdfpk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gxyyfbyse.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/ghbgwjben.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gfqqrcofx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjuevxlaf.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gwoizqjgy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/golsesfwb.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gvcmwlnoy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gdpoznxse.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gmvbieqso.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gvdfphrwg.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gbbebwknb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gnqtazhvi.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gmvxnkqiw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gxptehekb.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gwvsmgmyo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gnnjkseqn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gmwojgszn.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gndjdbibh.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/ggclhxcqz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gjhdcsvdh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gkmiqfokf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gtdqbsgkf.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/grsjwlxpw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gvlohliej.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gzbjtpfog.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/griosqhlf.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gxkmmuokk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gorqtnkwk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ggxlcpogc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gvsfnisis.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gzmxmbjjp.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gzfycwion.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gpfvitbrz.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/garhrodqs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gvswzrrzy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gllmvvlvp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/ggvzhmyvi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gxjpvcdhe.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gpapdpfuk.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gkutbupqi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/getnvzltw.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gpdoruhll.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gcjwpfbnf.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/ggooikukc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gohenwxaf.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gjngofeoc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gbegyxeuq.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gjwwnvqsg.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gdjwxdogi.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gemjzzajg.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gyuephatn.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gechlzwpm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/ghdcqpzeu.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gtlgntlrg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gmadiftfv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glatodift.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gfqmqkozk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gspopuaow.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/ghpavmtng.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gnxwetxrn.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gnvwnlthw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gbotsymfq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gwdmqgysp.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gtfqltjgl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gidksvhfa.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gcfklbpeo.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gfoymoenw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gtnsrcyve.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gaevcvwut.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghucrywnq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gfteseice.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/guknbkrym.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gtnrqlbbx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gagatubnq.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gcievcpnv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gczqhguym.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/goymwnzkn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gruwptnhn.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gxahncdik.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gxggcjtxf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gxwxljqyw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gbwplcgya.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gykukijcx.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gcesuvete.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/ggjbysvur.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gvfyyqxun.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gxszjbxlm.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gvvcgoiof.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gpdtrkent.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gstfwuyqt.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gwrjdyrxc.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gyvjpwtnp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gyjcrplys.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gimbfpfde.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gdcvdcxwz.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gdibkyekh.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gskaijvae.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gkjoqlnbe.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/glrvjtmwl.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gtpgliqdi.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gknhsrheo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/guuxjtmsd.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gqdupxdeo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gdakvqpkt.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gorqnbuvn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gocsfovxb.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gnvhndgtq.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gchuofrug.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/giexzuhnn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gtoyitiok.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gpmwoalrg.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gnjslzlti.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gjbwxizos.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gxwrjvrhx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gexxmknzf.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gazoozgma.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gqamwcubp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwjecdug.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gufecysnf.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/grpyjjavt.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gvjovackh.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gspkwjjbg.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gkrvnsayw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gtrbguzug.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/geynqiwoo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gjicoylei.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/ggklvudzu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gogqisgqu.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gajhwuzkq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gtmuwslrh.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gakxoqvct.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gwgdmkctn.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gkyyrpmtx.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/grabimrpg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gbhrmhobr.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gxfcddxvy.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gqfkxydhs.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gepvmxcan.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/ggmvomubt.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gkcbosrcc.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gjiyjnznf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gdqxjoqij.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/guyhtdkai.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gomexjiqm.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gpktlxxsf.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gxchypfnw.sHtML


<!-- 参考信息 -->