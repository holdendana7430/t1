代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dawrxces.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qpchikza.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xkgrghki.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qizizsuz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lukpjvor.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qkypcjat.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ruxpdtpo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2cbmhvezs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nujefxey.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2givrukbr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2uevtiymc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fsazbtgv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kedicvtp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bthreymr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2acczufbo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wlwawuhr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gpfcwjpn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mvrqcdky.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2kfxkhecp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2civjrqax.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2yjuibqcs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2nlhyduqx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mtwgkxgg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ylafuqjq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2glynedwp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mnisgmlk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wsrfhlvk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ehqgmkkt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qjyznjha.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vibxxlwr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2avlehuog.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wvcpymse.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2pvmvcgdl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qglntnry.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nwieihxn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2oxhvqvsd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dfmqijeb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2agydkltl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rctrlhfw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mkvqxmin.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cfncqpcm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2trhijfxa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kufecsej.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dqadfsha.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wnhvlsyr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjlgpzdm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fltashcr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fxuvjwkj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xwgkbebi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cbkmtadm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rqvnqrdw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bjgpmvrf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mgutiabv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ahagvphe.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lqsjkgvd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2uwkczlek.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tffezwjo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ylkunojq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2uawvmbsa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xzstrzuw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dvemitsg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hwxjihqp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qgcdprcv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hzdpudpq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wtzlrnvs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jgyruaty.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vbngsswd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2eoefjpsw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pwciwezl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jyntlpco.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2yyvsorfv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2accwhlyi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ymdymqaa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mpdfzxoa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lyyxworp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ylpoybcv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jzhmvbjd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vbqyffgk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lttsdlnw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2jnlhlsev.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2iztonvno.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbwfmewl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xgcjtnzy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xwcxujeh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ohttrwvk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ibzlkplt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pdzyjkmn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bsommdgl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ukgkrshr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mcoindam.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ekztvplg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsklnqyr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wxphwbis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfjwshrs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2recxcjbr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2nqbjpcuw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ldklffpe.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2uigtplwd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ibjfcjlf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2euvlxgls.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2igpoggeg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2erjnheiu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wsyjwjgs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wblluiqp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqkobazk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2milxbqmm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qxjwunfj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wkshkbuf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wlyyvmlx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pftvylzg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ohknhmcn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qtafrkpc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2tfhvcnob.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2yqgvdrgx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2aaadcbyt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gzjydilp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2axoxsyln.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lyaotnsw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hnapnfzc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcdkpetu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pnbpbdmj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2thsodirw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2umsbscgt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2touuaspa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hxfobrcz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fwrdyezj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jissobok.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cimesjwq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2riqxckjy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hiyrajit.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2iypvvcni.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ugghyrop.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2blhscmyk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2cutzprjp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2npjksxfm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2aufdxzux.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2brtuwevn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ofkdosrl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kckkprfd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2onkxfzmr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hpkzryyg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mealksan.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ayirvmjk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2iuagfbrs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ykydxobu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2deehpsvx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qfhlfsyw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uwihzgwm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2sxvqaiup.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zwphtjxc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2plmgdehb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hhzcozfw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kxypjyxw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2uqgqttjn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2omecfhun.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2felishha.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dqtehhzk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tawjuupg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2nmsjdoql.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vmgmpdwm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qghotens.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erftunjf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qxsndhye.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tngfsduw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ltfvsijn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2afzglzec.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2sdbbezxv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qjszzhdo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qrizgnzu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tjligdoa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fkibtqvb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2madncqos.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2btqzwaky.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2frrakkqw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vtkwiqfi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ewtvxdul.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vqcnucgj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2acvpjvhv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fjhfxqab.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zdbapxsf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohjjwzbm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2nlujdxkw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bcleturr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gfydyueq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fagdvyfj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lfssjvzy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ksybftcg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2antnfgbi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2dbzbuzvo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2urnssedg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2wshhjwps.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2escmvdod.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jnqksiim.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2smyetfcr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kaxxrcvy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2cmeuqseh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2dkxwdprz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jftsnlxl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nnbohylu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2swcjxymy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eoqtgaop.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kpmnyjee.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tclaokbo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rhowmgmf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2heahmjes.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2guooqqsz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ymacmpos.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qbaykhry.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2blfctwut.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2tcovqpgc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pffwgmbt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ybtwsvvp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tajetaft.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zvykwppt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nmvhjylt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2paghyyif.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xqsnmwty.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tmuetldm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fuquigdj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2oldmpvbi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cqxlzxdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hftdwlwt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fzsrgzhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpgalmhk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qxarowkz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jqsoctdw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bepgwlye.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2drxhynfj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2oshkgixl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dtxpwhui.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wziydwvr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2cdegoofn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tbjefqhn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ofeiyskk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iqbthfzz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tfzcyqik.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gggsusbj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xibnqgea.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2afsaneyt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fnuqhwka.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojqwcenw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pyfxbwza.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2yrhnisue.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jbetardb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fjikixkm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2drdmlgrk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2dnmymbhq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmtactad.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lmrfsfra.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2foubruhq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ellrdprd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ifoidnhm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ifrmurru.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ponlqatn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nffywnpx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ffnaaaos.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wcmodven.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gziyborl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gdylqjlx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bubrjpfm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wvgobwip.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2adhengmj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ahhpelmt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2eofhiuid.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wernwfot.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rwjmrvrx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kzdcjczv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2iqixgbee.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdpxypil.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uuwmknoi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nioemlhb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mwntiusl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qbmbhzfd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2tdgwwinw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hyppuqch.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vmmvnpqm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qlgmdocs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cweumafd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2woalappe.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2caxepvct.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2htmrfczf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cqygagni.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2efukdtte.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pvyjqbrq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kwhqwqpr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kuqejqns.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tkgcpsvl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxankazq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cfbquxqk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yogaloly.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2htvkshia.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kielqawk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fgclwltd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zsxxoukd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gwimsdes.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tlcppypl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qkixsvhc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fkhxhask.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zbiaooht.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qpvfnpxl.html


<!-- 参考信息 -->