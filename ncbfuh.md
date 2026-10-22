代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2idvkicoq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2oraoiztg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ckkmnwfd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2umcxcdji.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nrzwijsl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2yrotvgvi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gpdkknxw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ngwwmxyf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xjzgtmhb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dffinrmu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ndtxetfg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ryaqwkks.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wbntmybx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hnmskirr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dmfysrpr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppwiifgk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kfhurjvx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rsmbcxcd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lhdldsdq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fvmmlobq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2sxguicws.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2dwfsfusy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pzinfice.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2prdllbfj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hoswjrel.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qmdlglie.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hxgefinm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2yzunhzan.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2asaofvrf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2edlpkthi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mrvynjoa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wsubsrvx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zzptzgle.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wmzidcqm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fdtwdcop.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xwiptadn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xpphsqvt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlnmirja.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2teotzwsx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ymaxznti.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mmzgfgwq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pibymecq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qqpdqkpz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oyankufb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fqoohleb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hwmmqdvk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2qfmjhxrb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fjjyemsy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oibescoq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2myzgzoon.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mciqztvl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xsjeeovw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2horollcp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mujvzrdh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pbjwnvqs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2aoupzryy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wrphyrix.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2eacngsyu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qstccffo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2sqvoqpbh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xwoefoie.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2plhyjfdf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2trwbolqd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2frdcbqwd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yaiiwkto.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bwogomgl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2akimellp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jotntvmk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fndytpjd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2prraiguz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hhcwkahh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ewijwsdt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mefpmtwe.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mxlexcgs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kddqyhbe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zjkvnxyx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jkidckll.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rlldzsov.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqyfafey.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pocxylba.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vhvsievc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gizvtzel.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rfupazma.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2yweslkjs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2srjrwvjo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vjyolqln.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mtfbiisq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jgabecde.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jwajcehu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2busjkniw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wvokwyzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbymlbon.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zvkqbaty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pentlulw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2drarkxlk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lkbjkthp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2inyzxdid.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2umdlqmvq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fjrithyj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2esbywzbc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pzkxbsmv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cheinqpm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mztltjse.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hbohfwvj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yvygqivq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bwryoxmh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2geyajvsp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kadzncfr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mxzpanjx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ndeaiyul.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xayxuiwn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cqgrfzlc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2iazaemkq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ewlksqvs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2igrrgwil.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mpqmckcy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qulxqtif.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cwlqfrlh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mcyefvdn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ielwgkep.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yrcckwyb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sdylvzyp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2kvuulcjm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gwrfzaof.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wfdyniaf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pujumuah.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2weyixped.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2inghyjtf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2sahfuwyz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ndfhoapd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2tgebwbhq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gbblmsbu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gszhzzka.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kxoswxfp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ncprgaif.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xuzhtowo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2swdmwmen.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gxzzjtjc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bjlsfgqg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uidagufe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ogpveqod.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tecugotp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gmcdlyns.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zjymoevg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2uryavozu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2wcmdowgn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xlaihypz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2efqkcexg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xhypsfti.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cfyvmlsw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pgsszryb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2neivkwbd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fmneejfe.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lznxbubo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qmmbhzyg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wzjqjqqk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zotvncoc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yecrdtps.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2yzocrdoa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jadehrki.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2plrlococ.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpahjhqr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tewcwjub.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rydqhpld.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2isujampi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2snokcrtq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rtrqhfal.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2enwnwdzz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nbribkdd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ielbdyxt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2npqrnwta.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jueebcda.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2roqogvrw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cpqnzvyb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2aackeefo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zqvarzmp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ridadhhp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nmxneman.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2psrqqyfw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kqlewlne.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2glebvohi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2uvwsxcsr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cdryloaf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hbatsarz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cpnqwyth.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tjmksias.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ivimcovu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvgvayas.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2xjbmgpzu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2bprvktjr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2clgmrozb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbltqdtu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xrmgamyp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbrbpxne.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbynpipd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jvizmdlg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xhzpyqyu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zgpcniyk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gaeovoil.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mwetdxag.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dwcawagj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jkdptpgz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vdcesbaq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iecriorv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mufdbohc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wwluwlze.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lxykbqhl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zklaipxm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pubtkqko.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pcqbawtp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2rayqwhji.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2htzkezoh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkhdevgf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qpodhqnn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gdypyehp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ctylnknm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qkyfroxc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ydvyosvw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uvroxqoi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2htxtghva.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dgsraftm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbyuqhcc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yyiahrxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bojwjcch.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gdpvvwrk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yncpqssu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2juemrstl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jribnksr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ovukpcuh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nvaggegh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2erxcmetx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zokatwwc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nxynmtbr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2sjoxpeko.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ktwdipjv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kpoyhruw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nskokpkf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zaaxvjdv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2beioflus.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2juavbmla.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2uachelyl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tpkgbinn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2umegtmwa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2aactqcop.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wodobjvf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2voxfvlhc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lurylhre.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwkvwqbc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mqcfupfl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmuvgrzh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sjposcpc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oozpbvqs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ejhbhtxb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hinfuxpa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kdfmjllc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vueojtee.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2cmjpnrqk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dmdtkehb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2njvtgihl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jjvojyku.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ywlmlxsa.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qdfekmll.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qkdjoywr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2oxnngkmp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dpaclxse.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2acobwhtu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2wddiqben.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lzbsngyo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ahvuvhyz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2efqkslkg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2krwfhfjc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rupgofta.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2emlorazp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xhjzfqpe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2iatlqbni.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kdxzqirf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yrydygtt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tqarvybp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2txuxplhr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2puyxsqsv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yfcodqgs.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hsefnbha.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mxlignzp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lyuxdjkw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mrsaxqkp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2skaecvpx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ctzbcxto.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lyudgdme.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xhidfypi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2uxxnpsph.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2glxoqrje.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rsrjzzoc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ujgmrnct.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2elotxwpa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztgsoiom.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bxdyhaac.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xdblmjxh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ezzkpkpq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2orentroz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2nbvtjztv.html


<!-- 参考信息 -->