代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xzqhsvye.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fkfiyuau.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2caxliuqs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2khsddhsu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mjhirtxv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hrjdqtcc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dcltbhmj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2aoqqzqor.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pympewkp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bfinfvjl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ydyhmrlh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fazcqksj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ktdcrjpd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kdkjdcpj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lbqsldfs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zxbbpvdb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yamtdaum.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dizcyjxe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vjenwdiu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2aykxpvyq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tuiigndq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tqwzzsas.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ozwfoqdp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cqgmklef.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xeujiueg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tuceaomc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hbptqked.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2govekmei.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2aglwjdkl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ammzqhfc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2djgbpddu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kvetemda.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zabfgfyg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kawjwbaj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2skklbfcj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tjxnyped.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fwsfxrhe.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kjkvbvxz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mgerwgne.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mtpigujg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2dxfkheny.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uhbgupnx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ygscjjtj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rnpjqguu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2iejfzlxv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2npnjbhbg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mlhaontl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cfgufyoy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fumwvczc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kloekldo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jfpbpgba.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oatglupi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jsgxyuwi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2otgiofyb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zmjktiaf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2trigzhsq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bdvfqwti.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uwtngziq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2znondmal.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2davvgblm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ctmhggve.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tbvfuoec.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xzccanfv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ioiuagly.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mrmoonwi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2bgozevlx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gfdofltl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rydvthod.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mgtqlsow.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dsinzzvm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pjsqdhtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvdjtccq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cnqfphlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wutpjxcc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pxkzmqdw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2seoekjor.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnhpyarq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mighadfa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ewggrffk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vqqtopvv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dlqhrawt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gsrcvume.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lmdkaygi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wgthibfx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbezpveu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kuoirghw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rdcbpcvj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pltvubml.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ccbszjsj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kmregble.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2uhrvkyxh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hebuqylf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ffyukkuz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wiyhuevf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tgqpzvdq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yzvpkvag.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2sveosyxg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tmudjorn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hscypded.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ihcdxjfy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tibymmzz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gptumgyn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2eagdogef.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pfwgorlm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fdetpswx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2oezjrxnj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2aynihgzm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kvfqkukk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bncxavtr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2icncsdaf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ocwtacrl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pgzhdfqv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wcfsrufz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dwcjbvuz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rlbwtzsq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rvlieirn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qlyycazy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jpbaehop.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xipfxhcx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ovztiqwt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2osguejhx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vxbcjhpt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2centforv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rafzhlhl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rvljezfx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hqimyiya.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wqpmsffc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ynsdkfjm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kmlwvrny.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2owrkpxwt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hwblqvjh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mrjryvxb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2yxigvuas.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqgtnata.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dlfcvuef.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2medooadu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2edhlkbrd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ynrvrxbe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dqecywhu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vayfzval.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gmeyniri.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qybadzly.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2uzzuybts.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ieiexixi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gfkrwsyh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dlggrrqd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jlqxdjrf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2micrantk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zwvfwqjv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2aricmnru.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kyduwbqd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ughwvoof.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gsixaadz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2kjrekhcf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rsgssoeb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2izugrkiy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zgewtuuk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tudyxknz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2igkzzgix.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2aryvgzgd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2maeunawy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zabzjqwp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwoxxmac.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vewsiaei.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hreldpyb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rjlbfxuk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2sfjrcowb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qchdnnrw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wyotmwsd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2uopfafuy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2orchcyoa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dntaeyll.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qydrwmwv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2bxvzffng.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cexnyces.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pivsbpuj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zjkmjpjg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucomgpbj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ncuwljep.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2eacatnfn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sgcdhjha.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2uwqxjcgo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kivfrjcp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dkysyskb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zcnqbado.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eaiiufjo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nbfgigil.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2oerytjwd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fyvvroyn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2obkmvtsm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ivuszola.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bwncjxpf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkuqgbpv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2dhljywot.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zmjcloxn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2njlfsxdq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hgueuzba.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2eluhayuv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dujrepgf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fjfandeq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fopnegqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfwjnfey.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ginakqmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qenvvama.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2spmmcsua.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2srywloov.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pfrrrozq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vdazqinu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2bethvsvg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jgfssgiz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2iilsfgze.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jfvxxzrg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qxpjhryj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jlwregqz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iukqgqvo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2naocqfef.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2igqmojuw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2crgwneqb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mziyxsfy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cpdnvywk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2nlrweyih.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vygphyfm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dbmhqomx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vrexjedh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xwnqeauw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rohdhyul.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2areltdey.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qaomtxbn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ydrjsnpq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhuezzon.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yhmcffji.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yujxkloi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2uotmxyxw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fxycmsgx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tuwmlvtb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wousomsm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2layuqbmm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2tggwgylo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uzcqiavi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2moewabdt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2njwtipkq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jfxdzmjp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zndkynex.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bvlltziq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fnqymbyu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kqgjrxxl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2irscquwk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hizttrda.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2igzobesw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nodobhii.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2snfzvojg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2viuqxnat.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ephdgflc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vhywihre.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zpesmtzw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ijgsfgmq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dkyntaax.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2lxxbowja.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lsvevhlh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wswqunrx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ditwyqmg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nadazfni.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gjgfjehb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dayfhwhl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2likcsrlg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nvnsqfqm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2cwtxsrzf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bxrvocxz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2poxmxykh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yozfhzvs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xdlivbjg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2krxahbyo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qmvnoyuh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zlionkuo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cahsiitp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zqlqzmim.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ejlgigtk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jbjlsetm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jpwfsiaz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2trnqbxvr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2blvcjcqa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qvtolbim.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2impeynkw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2uefitcne.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qnuknvbb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mbpzsywk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2njuvsxrv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fwmaguyr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gdmksmea.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2afixtvss.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dnqgtmqg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2fhmmflxj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2romailyg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwyjglkd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pxvjvvof.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ghrdaozy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rxwxmwwq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ygjnddkk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lbqhfave.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2indhsfzo.html


<!-- 参考信息 -->