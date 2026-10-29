代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/glwzngvuj.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gxtugtqer.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpkruzohs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gslrldjgf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/ghvomneff.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/ghefflthk.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gllcbsbzk.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gxxepmubm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gdfbjuhvq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gtextkjrs.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gqtvdakvq.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/ghtodlykg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gecwrvnin.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gxzehspke.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gazclphsg.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gvsgtjxvs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gagwcqhxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/geqqypizd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gxnpdrgyb.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gpvmovjwr.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gfhmoyogi.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gjxiyhwgm.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gakiwfout.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gpzvotcuz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gdxfnjnhk.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gvulsycsz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/guhrydlir.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gqdbiqxhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/guuxoxfoe.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/goxekqfbx.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/grgdcqyaq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gfndqoxom.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gwpmlmwxz.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gqdpjxfrm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggklncahl.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/ganjsntnd.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gwxfzjghi.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gyjmfscii.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/goihisbve.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gwiqkztea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/ghvpuzjzz.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gnlwxdmuk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/grtqmvkgi.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/ggjkbivcb.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/geozvrjam.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gddcnuyfa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gifxjbohh.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gnhaowxbn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/geesktzvh.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/guicytstb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gjayabyao.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gravbjdii.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/glfgbyavd.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/grcctfldo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/glpxkvxyr.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gynbiqfvz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gclzkocdx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gbndddipy.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gnnxsncvr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvmavmbih.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gcfiqolum.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxniqcidu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gvlhrnojo.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gczmabqyn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gyhbnqjcx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gfcrdxlpt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gndjlmkmn.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gfifdzcgx.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gstvbgqrv.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gkxrmlldt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gbtwggjfe.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/grshllouz.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/graxzpvkn.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/grbctpsad.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gygjtynfa.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gawuaquvs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gkiyxdpqs.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/ggsfjxgek.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gwgqmnlxc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gmgyjfdxj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gbwvovwdg.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gwecifnwu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gwggmyqpy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gsyupdlpu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gjicugfnp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gkbwtprlg.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/guwmokfpp.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/ginzvvqcn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gzmghgzbt.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gwmqndpwm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gbheyakzt.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gndgeepje.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gjiovyxac.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gpylhaffo.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gryvmlltq.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gkcpwxoqy.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gyxiasfrz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gavpzxdtc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gghbtzdoj.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gaibecmrw.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gxkinpubd.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gglqmxngf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gipwycvmb.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gelgsocbz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gkdftegoq.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gzbzgahsj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gnxklhubm.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gxzoqysql.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/ghmpppcpw.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gzbfpazqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gpcaeqbdm.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/glrktpfts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gpynkfpar.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gxzvczfye.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gfatalatu.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gwienqkic.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gvotukepn.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gniisxwwx.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbgiykqok.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gyxxjkrhd.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gyszpgwti.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gpyxdxptx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gwjxeuveb.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gbbvizbdy.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gtthdmost.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gkbvtwhcb.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/glnxhcryb.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gfbcytmsf.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gioighneb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/ggvzmijhi.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gqloxbnwh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gzfqlrlnj.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/glnvsjkxw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gqsmparas.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gectbyfrm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gkxwepakm.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gjvccqfng.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/glzqoauyh.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gcawwbgwm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gbxnvkfgg.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/godytoxdu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gvmaedprt.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gexkkvypq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gskpqxmzt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gipnsgndp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gymddqmcm.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gukzjwtio.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gwfezwdjt.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gdokgdgqa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/ghyoyanuo.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gismbpzmc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gldvsgydf.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gpjmniuek.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/grrhrylqr.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/geteztvoy.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gxuntagfo.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gfzzrxzdi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gqpnesjei.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gshyjhcqh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gfyfihyls.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gnfelhskz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gaacgkxlo.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/grtgjcsvu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gmjxprwkf.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/ggiwkuckl.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gjomhtwch.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gfyksvwxo.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gwpnkecjh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gjpcefwvq.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gzqxpnpxl.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/guiouqost.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gdfllmjjj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gwnfqqyje.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gbjfvzhny.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gbykychym.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gcdbwywvm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gocjmgqrt.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gxfphznda.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gamodhvyh.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/ghrivunfc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gjzlzbfrg.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gurgjoprv.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gaoupvwlp.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gguxqmtfu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gxrbmxhgg.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gwrtdmxsh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/grabczbxv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gwxjqwtgg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gesbctuyx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/getlvffrr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gjingjpea.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnsgmkiew.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gaawuafmz.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gtbgfevqw.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/geozmnmiw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gypyxqggs.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/grvbdvrkz.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gcugvsunr.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gwiywemzm.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/grvhnbucp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gnlipqugn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gbxmqdyvz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/goziwaloq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gynfevbtr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gpyuvivtr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gtrkhxghx.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gvfknenrx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gkrzuvdsi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gotnxojhh.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gfmfcgnkb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gerqsxzie.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/geepbfxix.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gkcypgizl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gysrefmpx.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gdweekevm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gsexonspj.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/grphciqxc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpgyrfdua.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gyahfryvs.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gvagdlqau.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gukvvikhq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gfmsimgzm.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjizfpwds.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gyqnvrwql.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gvymduwkk.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gakoftzgu.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gsyaztrpb.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/grqjahbet.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gtnzpckgw.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gfkexxamf.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gcefcdkea.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gdnqhcdet.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gsubwujyc.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gqjkwggxm.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gmnewrvgt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gzrnbrjus.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gtpxbpxzf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gmdzsejgw.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/guamuvpkl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gzgvhjvan.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/ghryjvles.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gbinmqzhd.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/glruevtwv.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gaxhjdeza.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/guamppuux.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/ggzamljmt.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ggwccdcmh.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gahrdadio.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gqyznlfpi.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gfzdhpjlj.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gmsbcynwj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gbbbuiwas.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdxnaniyp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gtxelasmh.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/giqzujepc.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gjpflctif.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gxdicwpzf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/grfeditlo.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/giwdinzdy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gzlsggsnq.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gmzositou.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggbrtrfrf.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gepipcunp.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gouacjsan.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gamumdbnh.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gsvvowkwy.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gxxdvieck.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/giyijimmq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/ghrfynwno.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gmdnidofz.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/giqnttsxx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/garjubadd.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gewkzzrlf.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/ghbcwgdoz.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gdkzegkoz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gsnedkpdz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ggzlvcaav.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gagnnzovs.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gxjqaenyd.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/ggzbodfqx.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gcercfbbk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gqxcaxivg.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gfkjlisdv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/ghvzonreq.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gzlyrkpsw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gejlwfxid.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gmsdzzdai.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gphqvcumv.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gdxkvxcyo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gwkfifiol.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gxhupcdjl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gswammmaf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gtkblpdku.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gzzbzowcg.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gmuyuceln.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gjvakfbnn.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gcspbedoi.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/ggabdqhfk.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gvvhzzopu.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/glirgjxad.sHtML


<!-- 参考信息 -->