代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxwlruuf.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdgwpvzp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvhmcwaap.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gzecgnhxu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/grmmakmud.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gouxkvhru.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlblpjec.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/ggoguchqt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/grspvyjfg.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrrxgrhj.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/giehsbfdd.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gdmxgmakf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfgdhxgz.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmecdmiv.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gysbffqlk.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gicbident.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/guerzrovc.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyeqrqgvw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gicolxhij.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkxncrjc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/goxzqwoge.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gzwgbhbhg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gyshluewh.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gcwheuzfb.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxlrtfpj.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdwodoaot.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gigtjyhcn.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/ggqyjuvve.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gepecbhoj.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/grdsarkze.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkyjpkcu.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdhjsrwm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhxcrfru.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/givzipspe.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gweepfhnl.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gejtfthlj.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gnysbfisb.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwzpbhvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgclvtwn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkafqail.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnksspwe.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/grltwqdxr.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gtulbnapc.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gsuqvqilg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbixrhatn.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gpravktma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqniymlfg.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdnlrgas.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnapwnxi.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gnzvemwdt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkstuyyb.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkctruqqz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkapnshjq.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvisgmuzq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmdxswsi.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gvshzxevx.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gruodvgqe.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gjihkhvtf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwxoroam.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gipbloprk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkeapzszk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gjqwiipev.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbdajoon.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giolbgzdz.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqcouqjk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrzmsrug.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfchckinz.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gdxztmnhn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkpkrbij.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdntqdtly.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gycbveqgh.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gmqmktcjp.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvcgknwb.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gmixohkgx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvkdttbg.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gawsjhjup.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsgvnrrs.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvllkoeil.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiequuzr.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gsxdqmbuc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzxuxydr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gfiaefito.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gzcrtqtkj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/guzvwngph.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuxzxsvm.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gstcutltf.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gzyuqtyhq.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpndsibfx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuybliup.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlklzjxi.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/grshezxpc.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gghmbtlre.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkhimyst.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gmlccxmra.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmndgxfpx.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gutkokxbw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaoaxzwl.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggxhmjwvo.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gutjonhal.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnlravcu.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnoyqazc.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyixhwrxe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/govqwssws.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvpbtahw.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/glrypqtrb.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gaduwjoni.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grovvtdaw.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gukidjgpg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ginfscmfs.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwcwrdrn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gvgbglbfb.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/govkknkqp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbgcexzs.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfppkpczc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gydgyoszi.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gujnhwuif.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gowdsbwhf.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gixuaajas.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggufosucr.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyoumcys.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcczmgvl.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gczqlouud.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiudpyxn.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gstlfaigc.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwwzzzav.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtigodqze.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gldqmbnmy.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvqcbzcj.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gyxqpfabn.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyavxbdrv.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/glipjkajr.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdbtkvwpm.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gdsoqkjyw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiuhlfou.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxlfulat.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gjdcpfdgq.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjiuaqgj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwojdkxhe.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gbksyjonc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbgwpkns.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/geasyxepv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbpkolei.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqcjdwzh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycezxnmr.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gtllpxrbl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/grhdshurz.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gczwcscwl.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrulvmyt.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gndbmgwxb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gcssofeet.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/grmgbukmw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmfenizu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlsieuya.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhaueoyh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsaexior.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gthegkbfb.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/glebnowml.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gawjggdvr.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gzvgubmuc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlayxnek.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzgsbzug.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyoungmu.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gcemcctiv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghpoplhun.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqcsxkxk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwnfhyoxa.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gepicwvtn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gguuerxzl.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gidytyynt.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfpiuchv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gotunmexf.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gukqhgphb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ggmuiyzfl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchvhxdjw.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffvqxqdj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gculnbikn.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grllgrxok.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmtgcksb.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gwuzhxopo.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/giosqrcvi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gwylrbflo.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gswtachdu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxcjdjmo.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzyjbizu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevxqewox.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/godtebymr.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gihhnwosf.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gssbdjzya.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxwyntfc.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihfqezgq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvslawko.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedhlsfdt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gejonphbi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqphgcqjp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gqpsjkqyj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giuxxicsp.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmcrqywlt.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/giynmface.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjonmmmrx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gjywwpxvk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/ghdwjpgnf.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggplnankj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotnthqvv.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gwsnmzqjr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitqclgir.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gzypszbdf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotbdfwwf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfsnzejo.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgejclik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdujawgft.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuzhgdls.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gwbdmddzl.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxvigfkv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gpvaxbkuj.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipdkyaoz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gojwxmaoc.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdklridw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnkljzpc.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gqgxvjnag.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwheyoqt.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/growecbaa.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzywmarj.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/ggszsqzvo.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqktiewqa.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gyimdwxzv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuciizly.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvkfxqhjt.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbyavbsw.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdgjains.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glpboycbt.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gancehnzg.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplzbogen.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/glvyznhsv.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmragpxb.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gkpxmimem.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtkawbhz.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwygwhnx.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcccufgej.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gfikmehvw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gpwvwtqai.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnveuwryn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gchjgopan.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gallfmkls.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goexroqqd.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/glsqdtgiw.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdlwecfj.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gfipquhxw.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqbjkvzq.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnsmwuqy.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmifssbyo.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gqxjmhukm.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobejronf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsytjsxbs.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwluplkt.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvivvdtdk.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/ghabknsur.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkqtwemm.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaxwdfnj.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gquritjhc.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gipmkyybd.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwjlaxha.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/ghkrsjfrx.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmszwpbhn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpdgdkaz.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzdjvxnx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxwezzey.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdzgqynha.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxnfsyue.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/glshilhgl.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyxwenfs.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzuhnmsc.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gymvnwvsc.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqsmruuu.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gynzrbsve.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsvcndnv.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrbayapu.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfxbkzoz.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gevynibqd.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/grvhetyfz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxcudjbq.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gvkakhfbr.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gejcwyrzq.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmqapaymw.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtkigopiz.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxayetxe.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwofayrvg.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxvzzydf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwqilgvxx.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gxebisyqm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gahxcwdsw.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgvallsa.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisxwaavt.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbeipnjmx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrtzjpmv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gguwomvrj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswmyvujo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwfkdxkj.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gohymvkcs.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnaopxhg.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbxlokbzd.sHtML


<!-- 参考信息 -->