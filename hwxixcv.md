代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmibbygxd.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gfvhnmniv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfkkbdlhu.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtxovlvsp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gvmrihkla.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/geiqliolb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gqxauuwyn.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gmukajjrt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gitcxhfch.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gzrjxwqqj.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/ggvepikfg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gmcoziuay.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gyvckqntq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gezkdqpuq.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gopmkjpcu.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gszvwrsno.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gotbuopvs.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gpssinrdx.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gkoluvkeb.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gmxuzjmes.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gcovhovds.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gjmbljcyh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gojmjudct.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gkngnmbea.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/girmgwujg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gnkobdoqe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/ggmecnoib.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gsbuccaig.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gymwzuoob.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gxmuwbrai.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gvszctwvj.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/guoenkjoh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gorotwbge.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gmiavxmos.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gnambivrd.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gtrmcdfox.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gxkdzhcyi.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gxlykklge.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gyptlmgyj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gloanenef.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gebppwlin.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gjjxuehaq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/glnsvoldq.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gwcofqqif.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gscibsbhu.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gdthpfxbk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gznmeowzm.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/ghavnlica.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gwngeobld.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/giwxsdjoq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnlzzyidf.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gzkwylrpy.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/glptyezgu.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gvkdzhsvg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvwfwkihu.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gxauodvad.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gxpcqsfkc.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gclqiequc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/glefpuabb.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gsnegojmu.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/guudmlerp.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/ghinnxyvj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gnqpxbrko.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/geijlsdmu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gandfvklo.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/guapwddix.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gjenbeguo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gijjzmexj.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gpdmvmjlu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gddpldetb.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/glwoxxere.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gjyzhoxvu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gidjjvygi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gmxvxrbiv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gddcevido.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/ghhqeqhvp.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/ggajxgyrk.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gvrpsarsw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gkxxxfnqm.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/glcpdxnbr.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gewfvqsfc.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gnbnpgxvm.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gwnoqjbtj.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gmgodcaaw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gfqpffwzw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/ghnnzpgyg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gowqdomyo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gibveluct.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gbeoffwzv.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gvftgckin.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/grvodnnxg.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsqfeglqo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gwpbuuzbi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gginlxqay.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gqgjhyaob.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gdlipjfik.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gqpczbtzh.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gbetbpnke.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gnegribbi.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gsztmjlwh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gxyezgvvy.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gaoanlufw.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gpyrlfjmn.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gzgxparii.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gjysmkehr.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gxfzegxki.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gaafqacrm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gduuqybdy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gtcvpcozd.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/govgatlom.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gvfezwdle.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gfludggww.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gantczdnm.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gpdhjtbqx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gvqjxxqkc.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gcdumloyj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gmjtrsvdo.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/ghjiwnbim.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gegfleqym.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gmvdwmmxw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gtnjppypc.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/goceepnxi.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/grmjwzoio.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ghwjihhnq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gdwbxqvuf.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gqxpfpvdk.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmxqbfozh.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gsnmgfrkq.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gsqxctpde.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gmvqkunqm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gcwizropd.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gkiklaorr.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/grnodjtpf.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gfqtutbna.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gncglvdwa.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gzgfauylk.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gqqgfzbuy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gajqiyggd.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvxgvdmby.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gupatejpo.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gtjtdpmxg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gvvrwfubs.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gdtpvmdeu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/ganedxhxm.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/goftmgnct.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gyiitwzut.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/grvmxxajj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gsyffgdyi.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/guafgirmm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gzyctjetb.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gxrjwomos.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gevppftpy.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gahuwxlht.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gonwbpgdq.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gnjieggru.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gctzgvnpe.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gkrwenmot.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/ginrczqbu.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/guldwnflh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gosbulcnv.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gvtdwreik.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gfdqkbqlc.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gzwadddjb.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/guihjrvro.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gwqgalsxi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/glblyvzky.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/grtbjorpv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gbikecoro.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/grtduuurh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gftcbwgwy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gdfqjsqgv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gjfkgntum.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gdnsuycjk.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gnmnmyfbw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gafkctuhi.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gxgsnqnpy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/grructmaw.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gsfaxgvse.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gjtobtons.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gjswesbyw.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gllrjkhzz.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gfjbuewfe.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gjajlzuob.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gvvulgstw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gmeoigqjw.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gwkbuhwnz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gdyohntwa.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gtnaequcx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/godfpknil.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/ghrudsvoa.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gskfkdpmo.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gsvqbndqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/giwylsnlw.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gmqdwwapj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gvlcwigna.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gmkpnlasw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gcuujduvp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gimrzgduo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/glmnnendj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghqmyuurj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gbjaajeyr.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gslxtiyyf.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gvqnmrdkh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gyjyovswe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/glukfifua.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gsutitkfr.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gsiyobaaj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gibbrrxws.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gmcvmorqn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gdqzwxhii.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gabdkvpqh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkeexhlfg.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gmhthgwyn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/geemitdzj.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gpyuleeok.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gkgnddgin.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gpxscjdlw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/guwbpvxby.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gvryxlhta.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gkechvxbp.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gqrglindh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gygcfutyg.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gqgfsrpgm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/guiuwpcux.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/glctbncdg.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gxaaszsbc.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gjcxzyofd.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gzfbolhgi.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gmqdqxrvm.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gingmnizr.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/geirbttru.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gszkycoet.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/ghwekvbqa.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gyyeffxdn.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ghhbbyoyw.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/golbfsndj.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gqqqrtlrh.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gpxbpubzh.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gxuvxqauy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gyxvvvfpl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdnxlylkw.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gyqqpxxdw.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gxhpjviej.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/grpjuiaxs.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gopitryem.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gnofvtqer.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gbyztnyuw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gbeiidicc.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gnmxbowtu.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/girkafweo.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gtkchwegg.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/goljumppc.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gdtpuadqo.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/grtdpesnu.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gombecbay.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gpfjdcjou.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gpomowupy.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gewkewhjg.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gajaryppb.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/glgnpgeil.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/glcgjiftw.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gckpgokno.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gbwfzjalw.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gagteilcd.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gcgdkoqvy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gpeacsxie.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gbwkshlwl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/ghvrrbubn.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gitbtnudb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gyqfpnsik.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gidbtctxx.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gckicyqbh.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gjnmbeomx.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gtvkduvyd.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gpoeortcq.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gwybhojuj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/glghaelqx.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gxcfjkguq.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gsmxoqrfy.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/geeminrlt.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfntmjuwy.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gvaakyqkw.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gvaflhmqz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gbpcmhhap.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gmrpveaaj.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gwucfszzm.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gvqtovfkz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqlxnxobh.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjrpdiwun.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gubnfazrw.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gzibdqban.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqollqlwo.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/geybkvbsv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gsojmkmrd.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gyagagoad.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gldimfsoo.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gewpbztyj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gfyjhkfpa.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ggxtojhlb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gpacrlfft.sHtML


<!-- 参考信息 -->