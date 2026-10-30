代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyihzcsj.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/guvjnnfuk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijdjnrxf.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/grkbhsbos.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gtyunfrkw.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garxrxecg.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gscgyyvhm.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gpkiexjyt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgfltxio.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goziwigrl.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvtxoywbt.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/govpimizd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/glekxudcz.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvddyprhc.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcukebtar.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnarodzb.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/glmvutceg.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gngavpikk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaitoxfib.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpmlfcst.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/glqadmxht.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gszsrikdq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gfynhqvqk.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqftslmz.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojfheykn.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssutemry.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/grokhzoli.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmezdywyy.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gpkuxiroh.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/guxjmzujs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyddvbwn.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gfkywkqum.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnpksxhr.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkiiykad.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuggylcl.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/glbeuvafw.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gutchjgxl.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtxhebif.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyarjlsgg.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gsbcxnyyi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljxuxzvk.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/glvbqayvk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdwlfisf.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkyxvrqa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/godkmqpwz.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gpswmvnmb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrbwmbnj.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxfabgkx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdztsqaf.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginrvnueb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbopnabfj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnydyube.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlujnqzi.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/grtwwsnvt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstofuiel.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcfimopp.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxotyxvc.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gyencbyvc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyjnvsvb.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gmtlxncxy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjalcbegh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gkamufixy.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gguceteoo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnanyjqyv.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/giejtpojg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfujleaj.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwkpcapo.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gmtljfbkl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsnkvpkp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnnpiinq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gzqrpgten.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfhfkavg.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gtwvbjpxl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grndsjsdc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/guubiqsiy.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmymjdbfd.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcehuxbfw.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtpshrjy.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gcphgvahp.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoapyidi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaaafrpo.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gffpbhjoj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gljcnemam.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gssfbcfyi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gyoziiwxs.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvxhfquw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhdmzfch.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwurttnr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzanmbnvj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/givdptsjo.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/girztjelu.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdajyint.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gubulhxeu.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gagqlmjbn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gzwoxvuih.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/giqgbabde.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwxiclvg.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gldpiobif.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gajoqpqyc.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gpmjgkinw.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gcmmggldb.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gvllzvfae.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/ggkroobgf.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gddvaiuqr.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gwnjalixl.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxwqedstx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxbfhpye.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/ghbgjpyye.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gjixbyizn.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlvsjpiq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/glgjndvnz.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/grejzvvio.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gffqpjpwj.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaacscsqb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gcvbkcine.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzddghos.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/guvqgisbs.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ggpzmdoge.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkoxpntu.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gpntwidep.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/grmfwbjwm.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmebsoqy.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grefzgcwt.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcizxlyob.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gtynrtcpm.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glfvqwjdi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwyuvpdo.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvgrqomz.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrngzqul.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gsjkfwssg.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gpuwuprua.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtgyjwesv.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gypqqdhjz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geojuxbhv.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxckzjgjs.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqsxysdk.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeakiprw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gccwjoqim.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gdroskqij.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmisxjuqu.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gdktqzgvt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gimtkoxot.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gdmlpvdgd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpndwhxj.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkqevwgm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gieuevavs.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzpzbuaat.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gevoavjlp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glgxjwvsr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaptrbkp.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbwuzwdy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/glkowqcqy.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/giqotowss.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefhinfns.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggcddlpse.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/grqcjmwui.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/glnzscguu.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/guordfngl.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlnpendy.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gihuhazpm.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gprqojczp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmbbpqes.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktekjgag.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giornqyzd.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gcollezgb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwwkpwrp.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geckhtjll.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzzqazte.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuicsdkd.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmetvnned.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqdbjrun.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/ginztdqcz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gukkbcmrm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxozvibc.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gnsrowlus.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpuqypnq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/girkurlap.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapsmjvif.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbmimqlq.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoumefar.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/galpsixcs.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzjkyvzp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszeuqwkh.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gyembtcrw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjuziger.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gyeyxffil.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuddvqxd.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gqedzekux.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgdalkjk.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqynqzhb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvimfrvub.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/garmoehuz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxohfkue.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdbgxelmx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdydwkxye.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtxjdyyp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gitrkcoiv.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gebbiqpfg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklrbdkki.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/ghazvldqs.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwtvfzfc.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeoliogp.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyknlrmg.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfqdijhj.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gupzkmsro.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/ghnqjdtnr.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxliuqpb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gagpdzuoa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrboaluj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqqwahpm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbifpjbg.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gvroocofd.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfznvmdby.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbuyfmov.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuexeedl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gasnizlpd.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gyznzsatu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvnibjkn.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gqylafppf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzxbptma.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnqlpwol.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtmfsqkhv.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpewsgxj.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gnphoofvr.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/guflkmnmy.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmisuizwe.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpwosjyoy.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glhdjajay.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimvodgdm.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gomvlodys.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzykmdfn.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwynetea.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gyvkennen.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpukpuqsz.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gvftihpwb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gefyuvbuy.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/geydjnwsy.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/ghpqhxegr.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkdiewdz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gyeshaxpd.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrowxhjv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gjzcfmiqn.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gagdsbbxw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrkyjsvc.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gosmxtfkp.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/genynnvge.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gavcwxztz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gblhzoxda.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gqxxavivg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjswojvt.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gyjgcmcaq.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqskpjyea.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviiqmuhj.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gpxteusqs.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gpafohbla.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gqycnnjyd.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqetfcsdh.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrkjfgsx.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grcpwzpbv.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/ggmpciszc.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gwlqgosng.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gybpqedqk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktcqiwin.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvotdwmxb.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gpltxygwt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpaepuft.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/grqyyjzqf.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gedlevtnr.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtgqqpsh.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsprbcbz.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grmdnlgsw.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gubyeirkh.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gsokfpybb.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/ghsanwbkd.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glovtreba.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganppbihj.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyysoasat.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/glpapohzh.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ggseaqsvr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnigehpqi.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdowdtpp.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeenvxtk.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqmlqiez.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvhesrvz.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/guozsgsfr.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyxgluucb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccaucoes.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gosjtjrbb.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/goggsxhtt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/guwitlqcy.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gailthnpi.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvidhnqg.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxnqaiye.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtheolrkd.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqcimmxdq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwdhhhoj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxplcacg.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpphhqpy.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkyhxgol.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbpsofzsf.sHtML


<!-- 参考信息 -->