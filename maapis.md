代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xhuufvmu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hbhxufgb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lcfrabjd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bctgmxxy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ddexjcbk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xuipbekr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kepbuzlo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3prrpslim.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3sxxfqhso.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wpimzdbn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zkprhesb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3fucfvpyu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vguszyid.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3osurnugy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3myxldpum.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3izlwhxzo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3scyhcser.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3npbzopzj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vsiwilzs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ettovpxz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wxhvdcdp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3uldvjgzp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fxjaxxkr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aphtmazk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dbmzxvae.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3syudyqsl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3yeuackqn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hylrjjbk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ckuwdlwa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3nnrdqznu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jfpoqisd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3edittung.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bwsbszva.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wklnswdd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nleqxiac.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zcskivqk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3phaqaqqt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eosldtti.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ontpvfzz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wmuqqccg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nyevdjcn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3cozulcwk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vhkwhogn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3seklvtfy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ydrcjaqo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3tfuickig.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ngztkert.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uozrtzba.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xbkpprbe.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bzjouicz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3czzgiwuk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yjctzthp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fnafmqne.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3viypyjhq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pcfaelgx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3istcfqbz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jofjualj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kedgnvpg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dpipnfgx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rmtrukhe.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3akaxuacg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fwcbxaex.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dphnevir.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ikxbhwjo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jtsunatn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3amiqdmez.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3viowxycl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grykqpki.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ccfllwjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfrpmftc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lachaewy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xikdpyzl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwgnlzl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sllizpod.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ddwhyman.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3crrxfuzd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zjnginec.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3aqwtnget.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3uxogonfu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zpyamwjg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3nmmilgig.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3edarcojr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dglncdcy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3maottdmj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ijqyylgt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3phonrwoj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fyjqpumk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3pcftaqon.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3plyievty.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gbcdstdc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3emfslgkt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vaqaypmb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hkgkmgxe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yvtpjfky.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3keatvyqc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pqkcahvc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vopucqcy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kfsqebhr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mgxlcxbi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3phwqivza.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3eanarqcm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3aehzngav.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fhpaadfk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fjlthdcp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rycvzujw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tkciuzvf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kglxzbqu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mxwpcfll.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3glzcmxth.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3tyswwmjh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ytqkvopc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tqvxruwu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3inibxbcc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vkbpfeiu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3elnzewhi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3sfvbanpd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3kvthjowf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qeyxqjvq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ewkrvlkw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kmstwflb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3abdpycjd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fvoffzce.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3yzqepmrh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pdilhjvn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mjdonqws.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lxpyxvbm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ppghvaqg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zqchhbxo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dqmsailw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3npgbejwk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3okffgojt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zxrfwodp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tcoxddcj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fqiaxjuy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pwtbzmgx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hfsspxeu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3eorbxcyc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ekfpmsjd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wnrzvqfk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xxotbway.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nkzbwtkd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xocddsds.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kukkwnrl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahfrlcqi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xwutlftr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wekotjne.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3oehsntvm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3csyxqvgt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3mgkaefkf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gcihrodz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lwdyamwf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rnsvlprx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3epuofyyz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fsfqgotc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uebddlav.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xrubwofu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tricsrue.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gmrafujn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrlzjdbh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ikbwsfjd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wqyvbbmw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bkbruaps.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xnwtifsl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezoozwle.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3nnjoreck.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3durfbunp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fhbxebnu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdqdoirp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jydhvfpr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3amwdchox.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wbneswsz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3svlpebou.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iykwbidn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgzckihp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3oijkmsea.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lgtnqqbe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zkpihqll.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cigtwlik.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3svzykfhs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3klqefcni.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lzzogtyr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zjlypqnu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3notlmbkn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bpgmcphf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rdgqfiuz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mlorqcsm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3sqdmmyab.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fxwjjgkt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3sihumdss.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ozpnldvx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pmkzzcwu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fpyzyyet.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zussbsmt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3piygfsbk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3goroydvb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mxzkuuov.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ugsweijb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycoxgkdk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dsjuseoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3witszcsx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wsiihvgo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3maytphrb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xcwzlofl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ajhxbstz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3rlnscyss.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nzfjmphk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pcrhtivy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3evoayluu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pjcvhmyq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ysdvemcs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gqvnrzhl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mkmjqdjx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3epklnery.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3znqceccs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3myabyiqv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ezzpqvpe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxmezqzf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3motjwkte.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ddkedydk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vrmjsbyj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dvfmprwv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vpjdkxfb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fntkzhml.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iikepdmk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rapcvmqj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvivewd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jijsmocb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jvuomqgj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ebuomrug.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pxfzzunr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oxrwwndp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bcoeehhz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3swtsppge.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pjlzmbva.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3spwiizqi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3esxxhutm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3exwucqeu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xvtcvvam.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tnxlkxqr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3enqksahc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qzvqupge.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zsyllcrh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3dhrsplbc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jmvvbdux.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmrlqvxk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tqonqfmr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yxioxqmy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3noejdlun.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pdnpjamn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3majwkwnh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nflaambx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tmwqfohn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ycaguiyb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ogrzjvts.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zzlfgkze.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3cekmxktc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dygyzapc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rztepezu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3woxczvrm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kghnmlrd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nimonczj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pffzytvw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vrwsftdr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wglcgvxu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gupecujg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hdtunfpq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yezbnwew.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hsimzzqd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dgldsyxp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pwbfcmud.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bggjbnqz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uqkosenb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tznpcnpu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rsdhyfbx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hxxumuec.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jkehrsic.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jkdrkctn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3locrlyhf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3agwrojre.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tsphjxpe.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jeicfjij.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tpmokzkl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iapsbxir.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3juqkbdqy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rzgbeozp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tpiebtqb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ahagmkbg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqxqnmwg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3hveqtycc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yytndfox.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dwhktzyd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fvpqwcou.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3emxrgfxh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3quixqzxc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3uideznfb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3unjmmujv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvxfhxjs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3avkaqsnc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3thlgavnr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kummryim.html


<!-- 参考信息 -->