代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mikumnzu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3docizkxa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gsqdqiuz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjiftjxn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hfxzwbdc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hlikbaum.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3yvexwjoy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3jqeeoeyq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wvyfoiyt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3eiuisicu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3npdivvlp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xbhrjzhi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dwjeofjx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yaxfzkkm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3btxddxym.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mpkgvspu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dnwzrvkk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3emecwlco.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rcycxbis.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ynsltqoz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3aofiuxwm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3newgeppr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qbgawoqp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pfjgrcwq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lazcumph.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3oygsrbrk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dnsytoku.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ixopcecl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qvbzshsg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fzwtnrbj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vxociyti.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jsasexoj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dhlzwntf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3pobhwcnd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3claktqlb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3esvddekr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3laoargso.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kriarbnk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vfqlcywa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wwblwwyi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wplapswp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3mqzfztio.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dvcvmgmu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mmjjxrfw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ogmztybr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3uxnjpcxw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dujmjgor.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qnprmfiq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ftjazjyo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rjiaumfy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cwhxmuoj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cbvxubbd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hbsuznxp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wrckpaas.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fnzycwoc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3rttilwnk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tgiltavk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hwtqdgwd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fxkwulmu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bxiwramn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kdlcwktg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3iyptbqsi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pckfxizn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kebymgiu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rkocgprm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3feeudibw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qcknroje.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tjuhimaj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3lkvfarsu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqxcmacp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3opnywttt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3rbdzxktk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3byejkipp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gzqefaqj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3olzolxfw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xwbvfdlu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3gahrizrd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zdmflzvs.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zpgitkqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anbbbqzr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ouyfqzvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vweszlbv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xjmievrz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wfncuepn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbqrxdju.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gpikbbzu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3hxbxpaev.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nipluunu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kehlmnbc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hdbbmslz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3opaeiumi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3knhtvaxf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gqamuwtx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3byroascv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3dxrdatrp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pnvgkrly.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3sarfxvlw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zavxqmza.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ddvbhagq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lmpqvbsw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fsctejua.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3uadbtlvo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xdmjtxun.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iiyprvkm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gkpfhfjr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zkytdyas.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vrekosxb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3raypatuz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pbiurqsp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jcgdvqma.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3unpiqmoz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dwahvudg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fonnrvlt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wmptdcsi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lrdnlgkm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3gxhldjnc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qmdalizs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gglixeug.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ujzmhzax.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wspxsqof.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qiwyjfqk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nrxvolon.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gujfiriu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pwvzekfp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3viocljqc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ypszelod.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zvvluzzu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qaxgfxqi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3obxhmdyd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zyjuacal.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qrtokwwc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sydomcbt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3xborhvql.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3itvaecdf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rzosdduf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3oqnjmnmj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3klqjmhtz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3owpbserl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eyfbcqju.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cbrafzsf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kdwniobk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3stiavuou.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3elmgouyj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3caxlqswh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yywwfqhc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3iuccaywr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qjtdtpzq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3byweegqk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3seuoesox.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujlqbqyt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fkpjhzqc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vrdknguy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jruejnfh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wthgqzxb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mlavctkw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3mjxddqhe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3owscectl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vubxjlyn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zfwsmvjr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yrkcesen.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3twwefsnx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3khhvyuwa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vkszqmby.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kmcicuix.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jkmqfimo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rahpdvyn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dyzrnoog.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eixislmq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ennmiqtv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kyjivczo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujivxmom.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xqzvgabw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3gvafyzvc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3edqkmjin.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gqqkxkgz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyamzoge.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yaiwzjle.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3psyzvnfn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yoiozspt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wfeghxrl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qckdrcgg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgvygjwp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufmipogh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rjamnmkj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3snnavuze.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xiuvkpix.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3migchcxh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3virdibss.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jgvqlizv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ernglofy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3whynzcme.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3pyexvuqm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ucjlvijt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vnglcdit.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dxcbltuw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mckyaxdp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vylxirdw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tdlchzli.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3niixlwmm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hvxitbub.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nydxdcgx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fqronfdm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3iwhnsqxh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3elmziquu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3akuydyyl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3etzsslgq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dpizogja.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cqljtwcr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fthheitz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbdbiaff.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ajaabchh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rigmzqfe.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pjprvssw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dzgqrgcq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3crmjkrly.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lemwzhxw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xtuymgfm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kwkwzaem.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tivorepa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gisnodav.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dxdmewcp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3djwgubhf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sxprmihl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3csatgrrs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3naptkuwn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lzyjczsg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ckxkabok.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dakajsfl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gpyjbhvg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fzdodjxl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdpxrpfa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3inzpxexz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3rjfglpcl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lvzupvgg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3iizitwaj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmgcjqxf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3uyxiuuyg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxskoatz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3siljjhod.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xnxvcuia.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fbamxlyd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3vnpxwheu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vovpaafn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kjdnohgn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rshiyiwl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3txlqqnew.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kzycpstw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3sbmtkzcy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qtnfgosn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3sttomtvt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3odcgqluy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3odlaewhs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3muofzhft.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3btkzcrdp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dobiwvfn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3stoscpet.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rmdflngq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kzxvjthg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wrmztpsr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3klidwear.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ewdjuglv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gbuupwpj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ijonavsn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3bxdplmfh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rxufyiej.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3smtcpmgi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3conzlyri.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bnbxirgf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rclbsccj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3teoigsvs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rtctgbvy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kehgnxxb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3maectdxy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cwthkanp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qjjeiwpv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3louyjvoo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3htiwoejo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ifslnlio.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3yidxuyus.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ujkekajs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pxrizphn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oijwshtf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dquhudcc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ofzbhirx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tltlndzo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3uhqhntxf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iblzkymg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jexhpdtn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hycaxqyz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fxqznwki.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mlxehxcf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3agpkkura.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rtrzyaxw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mzrxroji.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tuwzfycf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3oneowfos.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gqakrwzl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3krvnkcbh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zlsdetsy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lvhnsfxw.html


<!-- 参考信息 -->