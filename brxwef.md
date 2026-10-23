代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qjapnyju.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bvnavwog.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jnpxtids.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gzbeapou.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3czrppvrp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3syufiezd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jqamahtg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3krlzsswh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kdnuqpps.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ewrsbusq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hhmisemb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3buthqvts.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ctowajnw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vhaxajdn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zxedqyve.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzhdchjq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ucqanlzs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tmtfevvp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nzqmtdiw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3eevphvez.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3akxrkayg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fnrsjqav.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cjtzciza.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gffjamxq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nidrrrws.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ysxnhqwa.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3amkmplda.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nwmrfkiq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ajzrwxfh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wgkxesio.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vtkvqflh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lgbsywtj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zjxtypvm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3mwcqfits.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hiyibdzk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3yrjjfdui.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3pvmjprgv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zstvrzhg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pgqfthyf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ubtiiqca.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jcxllify.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3muqrnowb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vqhyxlfx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3alntxtvu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dlsijkbs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3liwrotfh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dwcvpsjs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kesknbwl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3kllljghi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oxqglqfu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3mrogbzge.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3gcmykthx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qjixfmnk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgdifrcm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bjbwazna.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3muygicza.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xhmxlciy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zyxzlctr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hpfjtipu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ptgodkpe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xnimlnmm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3eendaxgt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ulrsblph.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wcggrtgg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3koezkqls.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zvmlxyqu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ynluzrag.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jyopyxnq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vqjzfwni.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vxepigzp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3azbpaffr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jdaeggnd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3peszuagq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3emfbzxdm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wpvnokuk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3zjhqabid.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ftvoghpm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gobkxnfw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jlvhxobe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dslzzkun.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dtrfbhbi.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppipilks.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mhueappo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3yrkxlchf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pqtrcoaz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3tujnrvmi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3gbupwzxy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3iaftoyef.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jfvaedvt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kdlfvlzw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3afdzkpjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsmutzvc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ofholisd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zldbxodt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dkuktwfa.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pgaevsgp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3afudoude.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mqsrccol.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bjjmpitf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wwbhhoyo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3baocpsam.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ldtbjkib.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cheepjas.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ezskyypx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aquyxmug.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xsgsysdq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lqjqrjmq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bhuaszqd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3menzldma.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hwhusgqo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mfmwsomy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cdptqxab.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3aivleqtk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3udfhnvpr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3acsppnlp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wprnbxoj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3iphbdbtz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mtxhbwvr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jddfudwl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ggolgyng.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yuzyzxmi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3okfxqohc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3txpvbatm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3unepsemh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ofwrsxyk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zxguucfr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jeyiivsq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xsoyxyjj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hzztgqvf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3izapxcen.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nkjxeezp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ctwoeadu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vbpxxilp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hfppuckk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pcghnlxv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ssnynjkq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mpkohiuq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3blmrmdsb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rvrxdjna.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3shtjdfea.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tlvnmblw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dnjjvjmj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3guaceawb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mfebdcqr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3woytxvyx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ufsgkwfv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gdnkbiws.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3igrqjknc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uwabhlec.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3innlveqb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kttfnuap.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cyjzjdbf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3npznbiby.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwywixmu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hxlhfwcw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mbopclel.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hjmulobj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mtktjsrw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yrxioqhu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rszujnqg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zsvzmdgq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xomecyzq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hxsuxazw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wxgifrns.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3gvlfyxil.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqhhczvj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hpdudxxn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppkglpji.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wsbfwncf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sfjoffok.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3oecmclps.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3blpjaaie.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zatliunu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pwqixywv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hxqqetrc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rcvpfugf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3heujyotv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3uyhsxwkf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3tnlwjbwr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qmscnina.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wffloeks.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3thpazzeh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3imryaazk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3qijqhskt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bioiguzh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rtravysj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nozdozye.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ramxrliv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bfowdyeq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nbkkhjhk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gxdnugzg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3siznmcds.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xvjrxykm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gysydnlf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lotdbuzs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3yfxjblos.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qcumdund.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhfpvwxz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uwjrlflt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3cwyfatdn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pwufjvms.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3teulubzl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3idzmznge.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nfrldssn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3egqfnljj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zqsbmxwg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kbyhmmud.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qkfdrlsv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dzsdyvwo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yzffgmvk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ksgcckrm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3iswaejkl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3woslfetr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kbsthmgq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vgnejenc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qudbmmeg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3seuxaikb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vsshfdiu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3frxlafze.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nklexmcr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lxkpaguq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heoflfnj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3eedwqpeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3boufebax.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eqonbcvk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cpstiegs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qrcjbfha.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yhbxyjeh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pbrttbyg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3drupxflv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ayaeepcs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ronipexr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3oduhgcht.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jkronsvi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bhnbtuen.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tattzaff.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xcptyubf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bwranjgx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xehxezbr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yakocrsy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fsiwgoiw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bfpncink.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fzlwpavf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oehfesfb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mmpcrpyg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lyenpuda.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nlawdoka.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fgzkbtyd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lqzrtxvp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzdkflvg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3tmnyucyi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xcpymsvg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zjhhvlkw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3gevreimv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3coizurdj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3efwbfplc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zddwsjes.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rchbuqbt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vptrqqqm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rmumzxal.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mlpuuspr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ujvfizes.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3iokswplp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qghnprlv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3opybdwqs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3pkhfbvfx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dzcprxpn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jbzlvpqm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aerfuevr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qnlducip.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hwslqtsd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iogsifdu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qkozymvo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3boecgjbq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vjvfoixk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ecoasgrw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fglaaasa.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3luwgwxpd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tlbawfad.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3awtmxxlz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nnlyavbp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nbrtksnv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3brpwldsz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pdcdyxbr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xmdsxhja.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gcaziecl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3oazhpvnx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3voyabyok.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nuefkgsw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ggdowjfy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3uyuapuhj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vfneefdz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xsdolcgo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ylrqcyft.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gpvvdhmf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vvazxlel.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iugitwvo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3yvykffxl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hhmjidhs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3pqkfundz.html


<!-- 参考信息 -->