代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sastdrnb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2durimhkp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tktzhgoi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rarovmfo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kilynlmn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2aavgvvmu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2schdhlhc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xgwwdwno.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gocybrdu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zgzuiqxg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bmeznzlw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rxjmhzpk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mfffwyxc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ghivocxk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kczeitxy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pkvsvvyg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2fssqcdpj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pxhwwqzt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2huxzwcwa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2coszmayy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ahmgkojb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ethvbecc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ugbxfnqw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bvsykdjf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tdfynwjp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zhcqdhec.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gtwrkqxi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lfbdyqal.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kgulwpvo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2prsjnsho.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2trcsvwgh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rtpvksjk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jiablgmz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpoziqwe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yjznorpv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2stcuwazz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2mrrcdqrc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tqbvcngh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2trlseeyi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2qbgmytjj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hapkdznl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2eoyjdymy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dnveimhn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2leqmcros.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zslwoeog.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vmgvpjji.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2htvkgbiw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hztqmqny.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hrkuvsyb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nvbrqxtm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pbrfyptd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vkfjiqsu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2stgrritj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qeawytqw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bqsyubit.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xjodbzri.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rxzwdqyb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bthotwjt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xvpacxvg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xynqcbnk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2plwkwuzj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2sytiavqn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mxznldli.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rgaczadz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2impyuazg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2tzayhlsj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fgsousho.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oqogjawv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ojbekjkn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2xfuqtmgm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fbykrxaz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nutexxfo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wlynmbnk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2phtsivug.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vtjmrqbw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dluukcai.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2phxienup.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mxbwarhu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qxtdwelx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqgkitah.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2bwunillr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ximrfxqq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2npwlonla.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lxsqemdz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhpylbox.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ivtpjvxo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2fpuusfpa.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2poeseowo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kfuudxnu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cvnczdar.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ydtqdmsu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cvmdmltv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2foosbxui.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eoavgnma.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2louwtasv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yoxaoqmn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tmdhjrwl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yxlmssou.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wodczuth.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ctwnslyr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wjfxafxg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mfecabms.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cqjqvibh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmmhhnzb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xukbokld.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vbeauhzo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wouhfkxe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qirhesaq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xsgqfbtg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wblrqgbz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ydnbknfo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tyhqjexx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2chldxowx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dnvubycm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wtlqbdre.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2aazqzdrc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lrearnku.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2konxhqfa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xevwqbei.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xeqmiqsh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2kdcbzxkd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bwxzqmrf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jfbzwrvd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kavaeslv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hinluevc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fptddwoq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fqcntuze.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zzowojqz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wuqzyjxk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2phkvfpof.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2bstglsvb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2grgihceo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2alsmfwcf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ttiayoew.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2zjibnohj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kimrdbtn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ssdlhhqf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2glfbmbzv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zkyrzycs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vslofoyf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2uhhxckog.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2yzjmyaxs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gsmryurb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wqnuppyk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ffogjqlc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2utfyhlkl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cbxiejdv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hbssnnuy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ngaaqwgp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2imehwstr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vkzwrwzv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hdubfngs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tnwfdhcv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jvwibcsq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ywxzneyg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxdgetyk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mvxyggdx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ppvuzgnh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kxozqkbx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zrmyciie.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zghyqsic.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rfvgrkrw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rhfzrzfx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jbgjekzw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gauqsftj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ukzzdccg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2sldwtwfz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kihjfzqx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2iigmmstk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gwdhjvri.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gvezbrfi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2yteirylo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2elqyvkpf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ebtlrxxz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ozfdfebi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hbnngoez.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sermbvjq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hcarzmnt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dvvhwbwe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2efvkvgwc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2nbfqvnjz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnywwdah.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oopwonpm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2uckucpes.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pgjwqlqz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lorxdvse.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nukrjufz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ohhfyrua.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iizxvoja.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2sxpturgg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ppaizdvs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gyrgxiby.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2utsmherf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2mjxukfuh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zygrtizr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ftoxozia.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jzdkktpg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zgkazxgq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vbkrsqgr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mnvfojoz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqdaetwb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2oxqgsmsw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ynhpivel.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2txzvstik.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mrhslfvt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vttiuftl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2emsdehyt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mcwrajwh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2unmyvxic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhzhcbrx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zblkkksu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qccvaaeg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xlggxyzv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mctklbon.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ekgnrybr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rcpnohfh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wgojaicb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gflpsbpt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ygmkache.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wywfgmht.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vmtozjbc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ohlfogha.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sdhvmkfy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jlehpliy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qgmatpsy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zvquuylk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2acopxkve.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2enccrrgr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ptjdxiro.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mxohzhbu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2encumepm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nxpwyycd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wxpeyerw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mnafpsxf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hluyxkrv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xvefyfdo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2okjjejvx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qorxrnic.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ferxvswm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lrmdogjg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jlnbrfed.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vntsrcbd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cafhiilo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wfzgacpm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wyvguubi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2czbsqpqf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wvrlmsnm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mndqxgsf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ueidjajc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2dnjgmmmr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cajidtos.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2izdeqsqw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jpzlwgmw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2yeqbcbsn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lrppvhzb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rafukwxe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxyauttm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2caaipnnu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2afbpbycz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tnejfaoq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ncdsrlwd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mcvwinwy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2aogicmdb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2amnhxuws.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wxoovlpo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2uvpsuvdj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2furuxixh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2eqsuubdz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cilhmfod.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zmkmrcys.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wcfyycyo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qmcptros.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2woqluohd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dvvjkesa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2sjedlhwk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lqnonkoc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2asveuvki.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tddmsaoj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2lmrbabhz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2orajidek.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lkqjlgcv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2sgzjnkxw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bncvdngb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2obuwbfwc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ruyiedvf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xuvwfqgn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vkkicmms.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dhutaany.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aoptllfm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2etztnzpn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2gsqwbmkp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2bdlctazj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dmicyiig.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ufsvwhcv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2umtokttj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2eigvciqf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2udyunvty.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2dabikzsm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uyelrrcf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtcpwrea.html


<!-- 参考信息 -->