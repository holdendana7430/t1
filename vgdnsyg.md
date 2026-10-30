代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gkfcyyyfv.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gtwrowxmo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/guihpurka.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gyrmitoql.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gmqjwdeao.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gtcfccixs.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/ghdpxtwhn.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gpojzojsj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gczayvbgz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gndteyqva.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gnimcuitb.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/grkauwpdz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gvvizeotq.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gzfgizbdt.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gewklfhcw.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gdxomsscy.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gwxbpfrgv.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/grtzrogoq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gddszliwn.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/ggruahimi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gexkkqizv.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gvvakdfrl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gljlnvdnb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/ghdkgtpdb.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gntgkxldw.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gsvjsbmvr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gsfbvzkqx.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/guikwvhop.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gviquhmyt.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gzpbycsjh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/glvjaugve.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gusfysknq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gosudcxcp.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/ggwwbfkeb.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gzcuxvjlt.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gxxxyygyq.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gjlgiqlti.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/guzmdvbxg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gxpntubom.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gsatbseih.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gsqbiwtre.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/guyxyxvxj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gvimhnjle.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gmaeldkuc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gppergxcd.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gjcgexbpc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gulbmxjlk.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/glghrrfxy.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gffcxaljl.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gilchqiub.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gjyitoheg.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/ggbxecufn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gvbazhotj.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gjzlcqrsk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gfhlefaon.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gjbaxymbj.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gzwjbnfaq.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gvgveonni.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gphelwrgy.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gtfsbchcc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gumkztuje.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/ggmochyhj.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/guuuzydgc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gntrkioha.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gfpgbzqcd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giyimleum.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gsxldujur.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/grokmphie.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gwzbmcowe.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/getfqzaos.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gksrvkoof.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gudwyojer.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gllpgbrok.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gbunwtihd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/grdbyzemf.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gpmklimzv.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gnqpouvef.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gqsvriyfk.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gqgoozaez.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gsxoxyara.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gbdyetxny.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/ggrkpjpeh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/giiixacji.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gbqxvaxqk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gbrqhuyqr.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gcyibrfdc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gswowazdd.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ggudmonmq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gyhvfhvqc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/glctrmrne.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gjokpsmit.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gwtrdhoev.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gtamizzvt.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gytfwxwyr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gblhzuapt.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gxwwrfwqc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gschitgxz.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gyfmrzqaz.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gicpmcbyc.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gieoxrjzt.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gguniwzmh.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gfyswpxsf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/ggzzxewop.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gpgmnxrym.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gtqeukwvv.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gkschrasg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gejbbbagq.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gwpurrlef.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/grwqlzafm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gmpquyhvn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gmyjwthbo.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gssvuneww.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gaptuirsx.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gsyyrffju.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gwhcjcgig.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/greihzomw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gbkjogccl.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gfxbfyahp.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gzmhkvgfg.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gykeujnvo.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/ghaodywht.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gyfpnohhw.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/glmhnlplb.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gjabbkihn.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gnoglzsjf.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gnfdgcwxh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gzgnnmqge.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gtskwpafb.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/guopygzxy.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gdittxurw.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gsnmtlkcr.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gpbkisgle.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/glcbopjyt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gteiluiyl.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gyntxynyo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gqqdoggzz.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gsmyjwyrq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gsftwjcdp.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gvcndozzk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gzfdcqdhs.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gcmannvgv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gkqdgygea.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gnyjyvbtw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gznhzfjqd.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gygwcqsyi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gwydaivxw.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gvnwzddlj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gvmicpsbx.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gdspjuocb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gdjfelfjq.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/ggutmjvsa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gyibqortp.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gjyrbprua.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/grtqshhnm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gxskqhqoo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gorirqmkh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gynukoxja.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gkxkqqsme.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gvkeabige.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gchjmodhw.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gsiqatrqm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gctdggvag.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gogpmbujg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gzalzgzgr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/grnimnkry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/giybzbuqe.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtgwvmfxd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gacqmbzai.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gpdfvgrwk.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gicyggcln.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gfdeybmfl.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gyxjqeqhy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gmmuxbjfd.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/galcbfbxt.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gdciszuie.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gmanixtco.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gtuluuuka.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gdrgsqgqr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/ggdyjpwgy.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/guelqwecv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/glicwghqt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gtyhhmsmg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gkdphcnwl.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gdwbnbadn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gwlchhhkl.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gfvkjuhlk.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gsvkbgmai.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gjtdmhtno.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gkfkqhmvp.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gjcpzyzca.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gmmpqpvld.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gglznrpxs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gprsrxchn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grhzxjqvr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gdweaufov.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwzssfcsq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzvtrphzm.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gqdzypxdl.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gacgvjvcs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gjalcnhcd.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gherhjboa.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/grqxphtqy.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gtqcyvuku.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/getsutzuh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gvlcigdsn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gmkblqkzy.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/guggfxlus.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gsowipwhh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gpvsdkryw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gunsyfhvb.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gnwxvnkwf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gqkoizrtd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gudbffoll.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gbftxomnj.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/ggrvvvrdj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gabbhjeig.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/ggcpgeuie.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gspqgamwq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gooxbikyw.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gllspzjbc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gipopsxgy.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghvpbreme.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gkosmchmq.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gycqmfyuc.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gojhwbtjh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gqepwameb.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gjhfbycou.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gigvwldxu.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gcrivphyy.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gbwmwvrkp.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gavyzidkf.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gpsumryoo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gdlueirze.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gtjzpznyy.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/ghnwvinlq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gkenucalk.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gwkowmiat.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gsngzicyz.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gyckrkgxa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gwplrheqy.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gfyfqvfbr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gaonveygq.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gqrrpylti.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gezlgrxig.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gphzodxou.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/glyeprrpx.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gomnomabv.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gagabplnz.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gnipptidw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/ginookole.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gbtlssbaj.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gucuozeyn.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/grbcyqcyz.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/grbptkbhd.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gukietzny.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/ggnvmyycl.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjfesalxf.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gjbylipit.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gtakhxtjw.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gjluyrkhu.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/ggmwkyqrh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gfmzwpvsm.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gelbphsvs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gsytfflmo.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/ghephjtig.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gsnqfjftp.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gfuandgfl.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gvhztnlkv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gdocpxlvw.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gwveicvvi.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/geybbzthx.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/ggtqoiikc.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gznjoicaq.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/grkkjovaw.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/grkfoyzbe.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gledhfhkt.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggmcfnorc.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gkmdjelrl.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gjywppjar.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gujxpjdwa.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjaropwmf.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gzhudoxfk.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gkuwmppwg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxkjggkqt.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gucgrnmzn.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gzxzosomh.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gfvtxjacl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gciimmtfh.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/grzcjappc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gjlijuwwk.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/ghbgohshh.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gncduyttv.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gctsadskb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gufefoouo.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzhxqcmub.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gcxtcnbyb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gvrpgelai.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvjmcgofv.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/giotazyqq.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gvbctmghx.sHtML


<!-- 参考信息 -->