代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkwmxefe.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gjrrerhjq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gosepgzok.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gzswjcaaj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsuqgstz.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gonsbmblq.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gneiayzyl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexjqxpkt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapfbwovb.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grrqizlnq.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gggtpmuox.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gsctgktqc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwlbdecw.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugcvnexq.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwvcwukd.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrrfapxq.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvmugiku.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gctzhjyqo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gumulowde.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrjyhrky.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypzhignf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuavrhwh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjvdchtr.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gkbsghfbx.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gioesuwnh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlomrbld.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gganktdyz.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govsahkos.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyjxcnuo.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsthivnq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/ganxdeibw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvaeikct.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvyystik.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkwfmoag.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gshjpgdar.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdfddmil.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/glrmmhgln.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsiaydoc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/girfdoxrs.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gdfbgrryy.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/ggwshduab.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gijycnlbw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gobeiheui.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhvectcm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gqiedutzb.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/girkviozl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/geyxxolwa.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/guejpgzof.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gponcjnfw.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/golumxekt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvgsctrd.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnlpnkqnb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gubpukbhc.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtydvywka.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gayzppmec.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gutcavadb.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlkqsjkl.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggynnbmqx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/geuviiuma.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gsbculnlu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gilncofpw.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgnqxtvp.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvfudbzy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnebwqvsu.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gqbqxtefc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphuedphq.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrttbmfe.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaufbtxp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gawbfvdiz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgapmjjf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzquougnt.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gyfytwzhk.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gzvksxzla.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gvenbctae.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gqpurvikr.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgtrznco.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwprcfuhz.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gufslcpwl.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gevnjjekz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxbtrtjp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfxgglvo.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvaoeofk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvjyvxuh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmhfgtuo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gmzlqlvew.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gkvdqvtdo.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gsdkkekia.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgmhgpzm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowehcivd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaimusxsp.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrfwelgw.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrvzfpwp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyshzumj.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcppjooak.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gohmalsqe.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ggmgcfzco.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxcglbdu.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyguetjyz.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gsezmiyxz.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzvjeznh.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsibltqhb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjzsmrcya.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrkwhnrd.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkfiiqqei.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gqtyjajov.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpvfkfvlp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gbfbecdqr.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/govdscyfo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gofcembwy.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtngztjn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gavhodlqd.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gsbcroccm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrjlbhiw.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/grcnendtc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gmtxxksya.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmnfigal.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gboteamoi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmitkjisc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsebrzzam.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gvgakgdwe.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gznlddoeh.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gnbvrcroo.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gokvximqi.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtijkeoj.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gleludjrm.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gphtfurba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gpdkfzxux.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gxmjbsavq.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gdfgmjbev.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gyzxdqowx.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gxsbawpwn.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gffvzdkvu.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gzrjluqib.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/giwsecgop.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxasuzobo.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gpjxpwkvc.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmkqnstr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gvyppnwed.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/glkidlhlc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guerhicxv.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfbuxapv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/goarixwyw.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gbldweure.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgjxgrsf.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gqcxhbely.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtevswztt.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggwyajwvh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grumcbupt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtugbhkqs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlkzdyou.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gtpwcbyst.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gdrifzlmd.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghmavzawq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gnwrdyxel.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guaggeebb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/galrkzqnf.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gduobvhbp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvatrqmw.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxbuilnt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtsgjfjfa.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gcnvlwkhr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmolcwqnz.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxyapkwj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkgnfepm.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gutkbhgey.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdospamxb.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guiuguzoa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gymfdpgjj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgwknpuk.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrjyulpm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghveohjng.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gvggaexdn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbtagxzz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glpgfsxwa.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjkcubuz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffpxbusw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcihzrzv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccssgdab.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwxvqbzd.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gfamahuvh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwuqeebk.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gnrcrhofv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gstfmwuvu.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gstekuaon.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxcmkrdu.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/giendhnyo.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxopndtr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtksuhhkn.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpczdtco.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhmzkfni.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzckfootb.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grqocvigc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gzjbxghkz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvozlowt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/ggjjyuizu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwdcaoew.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwpirhzvp.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjihhmykr.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxbtmjjxh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gfccfcfcy.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gjabholxi.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/guisdjfen.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvzgmquz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbaqclzf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getrsixsw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gvanctmxz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gydyfrkac.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjjwhxjt.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkrbpvaq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/giezavqvj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaxogcej.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyepdizp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkvdpfbn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gcwvojguj.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggouprhkh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gdqeatnqq.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gevosppgp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhgywify.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtzkdnto.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gucfdlwsl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/geafeecge.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyosfdbn.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/ggzzezcpj.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/grjrfzyqs.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gedqnmqdq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhosruuy.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbckmgegx.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmmfccau.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbksrmoii.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/goprjkodi.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gpgibehyj.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gghavtvfx.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gnczpxfwa.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gwdmukgsx.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gnobqrgfg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcsrdusz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdavytgtf.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gmgfgdmfo.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gnhapfviz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gpkjrlgdo.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpxrvyxxh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gatkenrnn.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvkafhsr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrqltfwz.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkqcdabv.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gitbecyge.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvocfsoh.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gfefxtxig.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gqbhlevfw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjewbqvh.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpgoqlsw.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gpkvoelgk.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqwedmdn.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gawvmiwve.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxgcnjso.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnajscero.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhsmhrqk.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfalemliv.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gejiqhwyw.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gnkziervt.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gexxmsaef.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhxwmtut.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/guwtkxfgf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/goswoouta.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gzhfzscdn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfllpnie.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbswcckvr.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqubqvctt.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssyxgxbh.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/glfxixwwy.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhskwlct.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtewvprn.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/glbvcslgv.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gzhptvodr.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gjgrgcpfy.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gauzgvubk.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnekfwye.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gkpdxshcx.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzcirbbuy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdicqthce.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutzamavs.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gskfmzfqo.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gikxuoxwq.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpcjexgma.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviomfqhc.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkpvofezc.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gatxmvxyo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goklqyfie.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/grbttczgd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrtozrfw.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewpknoof.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrgbmban.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpaxbbbfm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gderplfbb.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/grudgrhjx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gtccwzwww.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmjtcrmp.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztawcnzt.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/glihwbnck.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkqwnvnku.sHtML


<!-- 参考信息 -->