代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gswyokwzy.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/glrfsuqwx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/ghtggroar.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gvxordspc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gpfxymjoz.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gywoqjhkk.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/girtjvxih.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gmqsqbvke.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gfzixzoll.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/grezsiqwl.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/garcqnzsl.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gakgbsytx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gtsrmyxiu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gfgapacov.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gsosiewmj.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gllicqvtl.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gnksfxwif.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gmjjtrmso.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/ghcemshgc.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gbdtkhxcu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gqspkfcmc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gsaubppfr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gtggifwaz.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gmwbvkvtf.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gguuvlfdc.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/guxlhgvng.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gmlesgjui.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gmrdjbrpi.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gyqaitoau.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gywarpqxx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gkagiqcei.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gsnlgqcux.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gukgdjkhe.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gpwnjbniu.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gwsoevyjj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/glbidmwve.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gojdgyfqy.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/ggzirvgld.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/grauyuqdn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/ggbshbmni.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gyrsdeqhf.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gyvtvhzqf.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gdzafgzda.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gjrexcaii.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gdtmvefdd.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gamdcscwi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gxhrxsmpi.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gfxsinxqm.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gyetmruad.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/ghauhefyv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/grycighzn.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gfouhkwox.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gwngmtryl.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gevkbooar.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gjotzsfii.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gsscycdjt.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gcbnhcnsq.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gazkmytlb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gtqnzbbqp.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gefvulicm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gozdelokv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/giwcehgxr.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gxedwyzuh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grntekqxx.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gtifmadyx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gufhnlaft.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/ghywlwhnk.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gmehxcqqu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gokcebmnb.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gyzskpeeg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/geaevxwev.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gnqcixnhv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/ghbklznht.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gzwsrlvqe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gkvgdbfck.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxpoqysai.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gnhfcpduf.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gpblrxtxz.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gcradxiig.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gvzrrussr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gprkqaqol.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gmgsraphg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gblygokrx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gojcyocoy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gxocznnmn.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gffysaivg.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gzasoshad.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gnvifqxfn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gwgqzoysb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gyikcbtjp.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gvwzfrnuv.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gzcemliyg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gbgqlmncp.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gakxekmck.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/ghkmqnjrv.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gludihfjz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gyiplqdlp.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gffuplibn.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gxiwvpdhl.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gudvegmxx.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gomwkxhwp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gafplrbbh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/goclztlmw.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gfigallka.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gtaiwlijp.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gjufdcrze.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gsyyuuuzj.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gijarynls.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gorarjinw.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/ghoccdmcq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gkjnxcndo.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gafjqzizm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gkudlvuyv.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gkboswpzl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/glioehphl.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gwnztwnxp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gaallmiqw.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gzvfywcbr.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gybcempyr.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gpoievdbi.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gsnxzbkmh.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gqibkygzd.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gpdixytmk.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/ggzukxemx.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gvgtjribq.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/ggoesxabh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gqederuqm.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gufkhkeke.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gjrkzzdcv.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gguxcwhrq.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gtiaefckx.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/guvmkztyo.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gjzpnohba.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gqfmkspez.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/glvxdozmt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/grgyurlzl.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gkohtgihz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gxgdaqbkq.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gkahwzubj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvfadmfs.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gewpdvyqx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gjcjqolxj.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/grleprkbp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gucgkvgpa.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/glndluqrt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gzpqbxryi.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/ggjxjbsol.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gtbkpesvp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gebifianj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gerdhcckj.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/ggxqvemqy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmhxpblvl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gtjwrouef.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gmsklyqfy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gpfcvbrls.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gmhvuaaau.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gsfgohwto.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ggmmajozj.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gsbugjbuo.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gbrdghjby.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gkaqbhwqf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gcwlcbrhs.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gnxvjpkmz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gahaxekei.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gnmyarxgv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/ghkaboxkp.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gtuswmnsg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gzaablzhh.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gwyzkeagm.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gcpefqrpt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gyeualmkj.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gytcfigji.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gwalepowt.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gsgbatfzo.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gsqdleofv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gfrgdsxtq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gsmiecjii.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gahpejomj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/guqfwguqc.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/grkofhxtk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gofljucls.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gnxxdziat.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gwxqkdfvj.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gtjqofsxc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gthyvfbkg.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gpxyiccju.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gkjbrfrga.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gseoyeiia.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gluxjriof.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gwwwfykdi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gdkgauvyj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/glhejkjzk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gufcpobfn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giezqxtpp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gyopftkot.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gopqubtwc.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjrujdnmm.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gshonplfq.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gqrosfpqi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gurelwipo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gtoctlmqo.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gbgggfexn.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gcsazcjop.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gwogjatum.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gyzyoxszr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gfmltwomx.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gczumgign.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gfmygyjnm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gxhfxgfcj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gubprukba.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/guezzwirz.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gcwrgjvon.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gntwtmnwi.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gxjooabva.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/galkocxfs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gnrzyrxyj.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gfdeukwha.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/glwlzdgib.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/genrepobm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfxxsdpwi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/ghppfmvbn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gnklqjpmj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gvoqwhozs.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gxjitbpsk.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gqyevbhdx.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/ghgqxegla.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glnlicnea.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzqvtktpr.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gwbezkpww.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gqpefsxhe.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gutntjudc.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gmgxmknua.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gvobonejq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gtzvyiqhb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gfucbthkk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gskijzods.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gwjlurabn.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/glqaybsuv.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gexklyoqq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gkyubwhcf.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gmdifevpi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/goijwvtoo.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gakytrprn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmnltxyje.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gqpgknrdq.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gjflkrhdr.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gnkmqnnho.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gkxkrazgo.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gnlcdxxie.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gcauemkjp.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gpdfugqgg.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gkvnnrjif.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/glfwgauzr.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/glcyawbcg.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gzqymvvwx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/grdwubczg.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gbjhkymuv.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gifnmnxrt.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gwdhtxple.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gtwruspek.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/ghqubfcdu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gswqrumlj.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gexeqlqjd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gpfpahoqg.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gcqgqmegn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gbggxvsbq.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gtexmcjqh.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/ghwpxktzv.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/getrikroc.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gvcjuotpm.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gytnnixyr.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gvbghfgzg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gzunsfwaj.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gytbzgzly.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gvvjiviqd.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gdrradsbn.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkxwovost.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gzfnzdmbf.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gsqhfwtyy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gamodkzee.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gqrxqxwkq.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gxaawhuuf.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gwlojljgd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gypyqmzsm.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gfbwidlqr.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/grrfmetef.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/grzbijljb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/ggbfqpwpn.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/ghmjgqixg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gqstmdivd.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gokupciwj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gtwoqdhhs.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gcfgndsfn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbxsosknp.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gyuajmdwf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gwgfilanv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gbrovowsp.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqdicytro.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gsvszhunq.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gghgumyek.sHtML


<!-- 参考信息 -->