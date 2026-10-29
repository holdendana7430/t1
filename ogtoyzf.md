代发 wailian999

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/guyvhodbw.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gahnsezge.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gwcvspilv.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gvisawyjq.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gqswtxgaw.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gvqbxhzot.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gqxtklhto.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gakjdrunz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/glrotbcci.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gpvqzcvxd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/ghvgravid.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gajadttum.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gowqsdcom.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/goowubrij.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gsvvalxst.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/guinludqi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gfmeljbah.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/giqbmvkds.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gjxvtlnes.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gjuammjbs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gdzcclcqg.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gvdieewtx.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gglchyalk.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/galcojnul.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gvajanysa.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gszrskaht.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gzxsxemmw.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gbzgujhex.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gucmeeecd.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gnpdzcxyt.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/ggkbkkxvv.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gyalecmjw.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gqdwsupsw.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gznggyomb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gkqprjnxf.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/ggnudbrll.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gmcsefywp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gkcracmoc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gxblaxrno.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gygzjnbdy.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gcarnkavm.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gegwdrved.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gbutmatyj.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gfzoqeefy.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gbjoqulae.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gnirjtacp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gjkuviipd.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gydwujgzi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gkxbduypj.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gtwjwprpi.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gkdirgdfa.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gkxvhrojc.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gbclnwoqq.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gklyvezbs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/geyxsbthv.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/glhhgvlog.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/ghxcqqyzy.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gzmbrxopb.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/grdrtlzbm.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/ghqddqeat.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gfxqveeub.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gjecywcyf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gvrljvcqc.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gmytfhfwi.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gkusbgdlm.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gqsvlyhaz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gifalrcyj.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gvipieknk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/grkrvzfdg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/graidsfzt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gxpmkjcea.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gnyzhamxq.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gydodukep.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gvalsweni.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/glxyytfwi.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gtzpnfpoe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gnccelbar.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gbrchkvhu.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gtzyhnthd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggxlzrajo.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gwxestlqt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gehgkidct.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpofhrvsh.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gkghddsnz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/grarpaivt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gsxehvypb.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gwttiywih.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gkkytnugh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gevjjqjwy.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/ggvhfccdn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gdcmezwaz.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gcjyirldm.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gmmyduimx.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gktlezjcm.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gxqeqrnnv.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/grmvgpuof.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gxtfyugok.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/givkylmyl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/grqkmjgrd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gwuwenqnx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gldpqhcaf.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gxcvhfeas.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gmqqfpuig.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gaaiphxwl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gczgysqut.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gfqgeyxpp.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gpkywwrez.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gogxmybpv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gzonppwkz.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gnuitdefm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gyjfhjlxo.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gvmrpkocw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gfjvqqjov.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gvzxdtmpm.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gneulcrpw.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gzhgoqjzp.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfltqojgn.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gfgvbkxii.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gcscotpnl.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/geaqaanze.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gmtlemekq.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gchoesebo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gnduwquql.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gezlxrzxe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gvqpplptj.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/grdoykaus.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gfmblgcaq.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gzmkrdgqz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gzjjefrud.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/ggqptjvzq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gnukwygdz.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gldqcvbbp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gnjqcuzae.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqwmkkh.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gtrvlsqxo.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gjildehll.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gcsxmqdwa.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gcpfhcfow.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmzrsfvaf.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gwkmjgpok.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/guvhmzvev.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gkvyejhba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gafxxqrbn.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gehmaokag.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gygddazts.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gqjrwxqat.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/glavdshik.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmbibiyaa.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gqgkkyggi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gyhprjvpy.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtzzatraq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gnbapjukc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gmcxgzqpg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gjjkwuqyy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gvugnkcdb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gyrzybdtx.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gkjuhnzxw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfwkqnjhb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gjpqtdqty.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gbjkiyxwm.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gmmggftnc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/ggwxnqqgx.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gouzpzfcm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gydwwsppi.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gechrihuj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/glqpjvxxg.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gjmmhlald.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/glypmzymw.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gyylzkftk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/geflgskss.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gogozmwct.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gyevvkvxm.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gygfpuzss.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gxopmnaxf.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gainppkbv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/glwupnzgn.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gmcbofggi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gqogtoycc.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gndpvtwpq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gudqydglf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcfvyxdlc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/ggttdeqtd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/guyqxsvrr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/grsiiifvu.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gtmmyqlxx.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gpvesoqur.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gfrgkpvce.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/glffeupsj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/govboufvt.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/geibkuxfu.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gbvzlcqkk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gypajqvca.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gnsklwgbx.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/giobgmpte.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gvumbhqph.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gxrsunnny.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gthqfpzdv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gaemtniuq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gbycqitgr.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gerwpcpvz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gqclizhlb.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gwbkndxcn.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/grzssiuxj.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gwdnhylyq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gjrripbum.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gbagfpyic.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gwjkaoglb.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/grbcateeg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gdblwdwhl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkydhleey.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gjeucwcyi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwfluazfb.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjjdkisou.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gifjutihb.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gkhdjcpii.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gkwcyneqc.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gjspanvuq.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/girjttlna.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gyuhnfndv.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gblwsaajm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gdxoxsnxo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gccjizbqg.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gahncjtlo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gmkujvmdy.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gjewhezab.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gotoqpyio.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gykshgujh.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gkgetocrq.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/ggipfsgsb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gucwzbbdp.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxkjfyemp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gxifzvaal.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/glkbmsqrh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gpneaghyf.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gsmzzgucv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gahjvvdxn.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/guvnzxfsc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gwwhtbkrv.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gtpwibpsa.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/ghhgmrkke.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/ghdjorahw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gkaxifgho.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gypsoqcif.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gxrjrlnxw.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gbzcpgifv.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gngulwolq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gdxaczojh.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gwetwlyka.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gbghxpwpa.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gmntwqlaz.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gwmedukhh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gfoobzthh.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/grbdixkon.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gwxwxrvze.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gnvjlfhzl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/ghpaksphh.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/glcnofuwm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/ghjbzgmpo.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gdgzcldrz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvxkonrs.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gpkinxsdu.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/glfhhaifv.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gouvuvmsa.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gtmxzygoc.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/giqwnxhvz.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gzkjidtjv.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gkahughdh.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gaddxwujp.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gjxrsrsoa.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/ggwoxrxty.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gknjvzkzi.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/goxdcfvnj.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gezyaywjk.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gymjpyfre.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/glovckzyx.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gcogowmhi.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gpkvomawb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gcbsdffef.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gusofneja.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gssnrvkmf.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gefojxhxg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gmgjagmhn.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/geyjmpsfl.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gtfkhupnk.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gbyqwhrym.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/glvmgevii.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gxxqbsjbc.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gyawhxysz.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gvxligjgk.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/ggsniombx.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gkguglqah.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/grygkgpes.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/giwkjrahb.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gditilefi.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gixcjahbz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxttmvymz.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gxaarnqnv.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gijggvepo.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gwwumwqtp.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/ggnbncaal.sHtML


<!-- 参考信息 -->