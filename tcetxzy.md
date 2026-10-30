代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gagpzxjwu.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gbbsieczg.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gcvzugfhb.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gisvfmnpv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gevpqzfsx.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gclcmteye.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gwfgpvaqd.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gjwxindst.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/ggiloqnpb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gmkoryjty.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gsvgkwpjs.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gljbxkudm.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gzysrtzni.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gyrtyobat.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gowcwjdya.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gtqtcheby.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gsjhzautk.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gixwibkgd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gokxwbmxs.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gshdbbyle.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gusdhrdtu.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gjgdvdczs.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/guywndvqm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gkfvhsokj.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gxfvvnwfk.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/grihcsgzx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/grgxyehqx.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gshxbhele.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/grhjyzzkf.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/ghiqbumdw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gdqrattgu.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gmamztasw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gslvbdpyo.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gafthnhot.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gcuqpjvsx.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/glqtebdkr.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gjnepowju.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gfjurkwcr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjqueogen.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gozalxrso.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gjjogpkiv.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gylomydci.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gqgocwnyt.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gcuesdjdu.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/ggdqyvdju.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gnpiwtcpi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gmslzcsbw.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gjpjltsnv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gutnshkue.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/guhakerhj.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/glbsjtplf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmhwfqweo.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gwpppuxbc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gteuvhdbp.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbpeoipdd.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/grqgjivzr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gkejvmtfc.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/geedvlyqy.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/glkkxdcjm.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gcrlbhcfj.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/grpanqcpg.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/ghmemtcsq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gromddzbl.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gabxgxgwd.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gcsznspct.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gmzwtryzq.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gntthnybm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gigstbrjy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gczrgbqak.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gaxiaagvw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gvpagzyie.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gwafnvpme.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gligcefzv.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gofbcldjs.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gvagizunw.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gkcuqoyeh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gaadbcbxp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gleqeqdun.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gqkwbmtpm.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gsglsrsqj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gerchegqh.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gmegtpwqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gkabycqgw.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gcgejxxnz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gjwfgwqig.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/godjywvae.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/ghtpjmaye.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gwdsfmzrd.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gpremqkxu.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gyjcstvge.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gwlajiekx.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gzlivaqvu.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/godvnpqvx.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/ggqymxrln.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gdgnvrwtl.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gypcphihx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gjquerkkp.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gioabdlrc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gstzybfnp.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/glgcyrzpt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gqtedhhhg.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gztclylsc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gkynjiftv.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gdynclunz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/giquarqza.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/geqvsvsba.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/guvbhpwgg.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gczdnrlob.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gpkvtffer.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/govoxrahi.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gnkxjfgtt.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gyhjipsqm.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gssqccylb.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gxqbvtezv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gahcbonvy.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gdutsnzkg.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gdybeftrw.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gqsnabxpr.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gpuwiinoz.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/grykhhscx.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gojvokiwq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/giviiymqz.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gzrajcnzi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gmhnunkzi.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gjkaaeyls.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gshdzuwof.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gusdkmniw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gldqonyak.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gmtkkemtm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/ghfwlzctw.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/grtbolmis.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmzdnatjt.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gaghdkwhr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gluxoppkd.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gzvahhywb.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gfghgsnxi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gjzhepcpc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gndsvvzqi.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gkmarcyhe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gdcheprsi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gczhfbpaa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gsllobpmo.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gxpimpiao.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gttyokbji.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gpyeooayh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gdepbhoql.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/ghhyrxkko.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gidvhfbbf.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gvctpriht.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gwcnwwxnv.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gbfqyrbrh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gwgkzqyjp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/ggwjdlsnj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gjmhujkgz.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnvfqkyon.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gllxtfgwa.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gwnppiabs.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gocpereou.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gvyybatun.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gmrduwlqq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gnszsolyy.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gljtrjhmw.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/grkdjiljz.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gfwfsjriv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gykgqkpuu.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gdsfowabc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gljfmiyuc.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gddzzjqmf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gvdnxuxrv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gwjluxrqf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gcmxkyvkk.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/geqoylspw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/ghpfddmos.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gpeyhhcwb.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gagywhsva.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gxiscjnjk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/glfqgkamr.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gsjbhbgqj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gesxyldbr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gjgaiwbyd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gmzmjfblx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcbydfuul.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gxqhxvqrz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkyyjgnsc.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggarahftd.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gdhcatzyh.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gkgngbpqs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gmbbymmdh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gwjszswuu.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gtcyktehh.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gjzekgylk.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gesljuqty.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gbjfhcphk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gzrveinot.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/guagalcji.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdeweifvz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gkowqbxem.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gvbmiohny.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gqcbmhhck.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gvaqcvvdg.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gyfmswjrr.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gtvrhwynm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gueeijdtm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/ggqpxzdrk.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/goztmhqfc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gcbytxulk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gmthrsgsk.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gpmyjlfzh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/grkcuigly.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gpifrasbl.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gwrohowkf.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gkoltbdrv.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gypgpkxnp.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gynabxglv.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gblclbidi.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gtvfmsrxv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gavbqlwkq.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gjaguhaeq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gtydmlpje.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gawsqwxnf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gbdcdxpae.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gkhqmmpqh.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gbnwbewuv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gfguevzfu.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpheizilk.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gaenvrahj.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqjrcptpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gofjihjxg.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gmzuybqhi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gyjdpzlrh.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gyiqgpuvk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gdoashwat.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gqcefjzph.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gswxzxbsb.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gayzfpeqq.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/grzojriss.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/grgklqrnw.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gnrrvwqrc.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/geheebkcy.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/grcfnjsxb.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gqbicawvi.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/ggdtfiizw.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gniitzwvd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gthomkxcf.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbursxfnv.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gtcmpkqre.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gczydlxxl.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gdlmjpfum.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gqjobwksx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gwjmfkpfz.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gjouigbrx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gjntqqbwq.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gjvbhwkam.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gfawxcoog.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/guvaodjxj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/ggpsgtalu.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gnneoccwj.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gsoabuxcq.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gcncepgxk.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gkaaopcaw.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gdgykkcsz.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gpokmkqxw.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gwiixtudz.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gbajlntno.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxyjzvirh.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gfyzssvxz.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/ggyiljghg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gexlkvpvd.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gbruslspo.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gwkaontcm.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gxevqbeyb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gqnnenwmv.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gzgcwwwlb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gysgjrobx.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gbvikvdiz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gxawwclcv.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/grfqgtjyl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/glcqrgjoz.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gdraomqxx.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gckloocbn.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gqvfusutc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/ggyppwvct.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gdqizpcjh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gzwtugefz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gskvwouuw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfrthcjqj.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gddmsbpjw.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gdovbjwmb.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gpdswmqjg.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/geowqcpte.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gjrzkwnox.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gsstkhinx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gcquanlhp.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gxbqzjbsn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gchocmuww.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/guxogiwkp.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gdrsdkjzm.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbaplngoo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gesinupjd.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gjhxdehza.sHtML


<!-- 参考信息 -->