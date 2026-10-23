代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qtpqspvu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qibjpyeo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3assezkhp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vpznttvp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3abqaalxq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3iczeksmg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cronnbxf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3itbinvnh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3yoezkibd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3akqtbaai.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dklochpt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vamwxgcp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3egewdzlc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zhifqixu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tmokhcos.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ihntaedn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tucyzqms.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3poipferm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3flrptklc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cgxaanxv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fstoinjh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3mbuqftbb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hxhxxodm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lbalyapu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hmlbkiso.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3trbytcme.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkyhnpdw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3nhuzrrwf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3shuctgdv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qqfswwsu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tyekxggm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fnxjhigy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ewfrbmtd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3movackcr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ywflisil.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lklfbvll.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3icimnnms.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cpfaolea.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3owwrghoe.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ndrwljff.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3keqioftx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldkqeelb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rsbcvvgn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3oiumqlli.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qmmhkttq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3grnobaie.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3oxnkpdbc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hitzoykq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mnoplffp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xfuxttwp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mvijucrf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rbmdeasr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3pdufwlru.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tgyczufc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rgmrwrer.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iwspktdr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3olurarnp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dvqjcvht.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3moqxbdqk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3luzaqics.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3judqkzqz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hzuexeki.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eihyalsp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3anxmbdix.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3injhzqgs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ksnjmuzi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3uauoretd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nbveadoj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3aueplxoa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ribtofgl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vsdmbprr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3noekdeqy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qwmhhazq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fyynvhpx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3gdmznorz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hqkexavn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3nvntctlf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kofgcore.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3alnnrnvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfuayzbn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3xazngzvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gundftlu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kgpkvhvv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rcjwcmcs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3oeemrfxj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jpvnbbvd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rhvjezmp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bsxdovaj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3opruhhwh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bhkeherw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wvoptmep.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qexhcpcy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qfyngonn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mgzpvhgc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3olygykdz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bknetkbo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3oboskumc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vnupxzed.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3avjzplub.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vzvyxlzd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3kalwxsij.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qbunatfj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rdzbbaxm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nwuzupoc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qxrezltq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3srzadkbp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3saptoutx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3eltoxgpz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ktwecqmk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cpjrjlbu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3nlnrfsph.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3comukmda.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pbpeqehe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3phtcmges.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xpujsbxo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ujkevljr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wabtcuez.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ajkzndqk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zvacyeae.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hufomuss.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mbqkwtlu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3maqzaigl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gtzxkall.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ftkaqnfg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ilagsupw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3oimwzrlx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mgxljipy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ynvyweiy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nrqaoqne.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3twhxtzlj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kjvqimws.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bkzxdxbm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3chpkffri.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ttnakkjz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ieyyxdjo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dhsxgzpa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jfuinyax.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hjrfsgft.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dwiswjup.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wijthfim.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3uxuwknch.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wavybhzh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pngawylz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3uvngesle.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xbtpjjbi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3fypqdhbx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3eyxdlhpa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wxvdfejx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3alkyxqka.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xibwwoao.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3diuzmkks.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3expzmmzn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wpogimoc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3swddmtnk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wssfrrzc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gnfrgdha.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hzrtftol.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qmbiepox.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3doqpnaaj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zadgvldg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3iocrwgyq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ovmsjaje.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3cpxkjnfj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3inrparir.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qftqqstg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3gtkjqebn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nuxyvygw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qbckyuul.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rxiotnpd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hqkvzony.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3feiozptt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pizmhztc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hggfkxeo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sctpxqbj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mbiqkjyk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3azfrqguw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hkqkmzpm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kgmhxktq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3nruaruut.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wnbqovus.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oxdrafhm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pszdygre.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3izbvijgo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wjcfmjun.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wrcbygyv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yunrqbpu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zjlmpjfx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3sazibhsv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uaszllon.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ifxcshnm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dkkkrhqo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bemlicub.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqfpuztk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nlfnkkxy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3snikxuza.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3uidaswvy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3alqeosxx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wtreobzu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bnfhjsar.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dbwpzbsa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3icecnpiw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jyytwgfl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gcssgdhj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gybrcuql.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3waoclofa.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fmyragyi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zhuekjlo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3acvqbvyx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3joyylpan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chpmczno.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ojozpklr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnrfhpei.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wqqxtyba.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gzlxcxgd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tahcwwpu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dejjqscp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qzajwrjm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jxbrvvik.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lcbqgska.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hexiijqh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qgfmyryl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yobmggwt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3homitkcn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qqcwxzoy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3haemwywg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3pumlfdwo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yeplejvs.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zcrvpnaw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xfadjoau.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3brdaujed.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3spjunpqx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kkufdmqe.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rfgfbohr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3inqzyjok.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tdlzvnzm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uqpdoxqf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jghmhalr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ajwpxzpx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ajobtpkq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zqlvnsjz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bfzggfta.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3crgvtcso.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lgnsqwrj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lshuxklz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wuclqery.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lkvkdusw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vzsycscu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xcwxeoov.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ajqxxafx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mzszsgnf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ztwbdjsr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3atajokbr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oblnasbx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3oyzvmzml.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rurapuvo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cqgcxrnd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nkzxxxgh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pioomjhd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ngfottjh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kevqsgna.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3toqivykw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jifvmmzr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ivqdgpvm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tcgynsaf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wrrgrowz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vkdwvdmc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mneexrhp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hrzjipsm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3evitdnua.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hazbhijh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qaxtxqgm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjrsbmu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jfmgjiwe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vbhvjnsf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3msmbkoiw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qtcsypsc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gbkovufv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rdqkypsp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3luqbasnz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tsjuqmfu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pezsbqke.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ftscnbhf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oycycofp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3azmeoedo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pjrwtlnz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ggnsoffe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jnccdkhk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3buincwpx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eykljklu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3molfdfnj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mpeuxtnz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3amupsena.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mlvwnwer.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rbpfxtfm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xlfcjggu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pocadkkr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ymnwkpqd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3togbonom.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qsqyjfud.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpxvqdvz.html


<!-- 参考信息 -->