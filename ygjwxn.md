代发 wailian999

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gthssbmmwy.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gticvipwrq.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtmtgtoctm.html

[R45] 批量删除
来源：http://hz.yongpay.top/gtrdmwgcnr.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtqckeyfpw.html

[R46] 递归替换文件内容
来源：http://hz.shzxlz.cn/gtyplosgyq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jlsjyb.cn/gtayownend.html

[R47] sed 单行替换
来源：http://hz.guowangkeji.top/gtrsysrdgm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sxryk.cn/gtzwyabkes.html

[R48] awk 取指定列
来源：http://hz.ivvv.top/gtnkdphxre.html

awk '{print $1, $3}' a.txt
来源：http://hz.sysykeji.top/gtpisvvhic.html

[R49] awk 带条件
来源：http://hz.chenzaomai.com/gtyqckgxjr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.haohaochexian.top/gtshatnymc.html

[R50] awk 求和
来源：http://hz.yuanzhike.top/gtgvrwcsbg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtcidvcldj.html

[R51] 排序去重取前几
来源：http://hz.cdnleiting.top/gtgqwaxqgp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxinkj.top/gtwyxgruln.html

[R52] 统计行数
来源：http://hz.ppjwa.cn/gtarnavsch.html

wc -l a.txt
来源：http://hz.xuanzx.com/gtlqbeulug.html

[R53] 查看文件头与实时尾
来源：http://hz.hammf.cn/gtfhxvhsgm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.snrcjt.cn/gtsecfritf.html

[R54] 比较两个文件
来源：http://hz.hywenlv.cn/gtjbelktxe.html

diff a.txt b.txt
来源：http://hz.0kj1m.cn/gtdshwhsev.html

[R55] 压缩与解压
来源：http://hz.cucudq.cn/gtjmqxmmko.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuxming.cn/gtfbaangbl.html

[R56] 远程拷贝
来源：http://hz.aizwys.cn/gttrlkxcjw.html

scp file user@host:/path/
来源：http://hz.snrcjt.cn/gtwxbrawul.html

[R57] 远程执行命令
来源：http://hz.chenzaomai.com/gtjpoqowzt.html

ssh user@host 'uptime'
来源：http://hz.birdmap.top/gtjdrmvbxk.html

[R58] 下载文件
来源：http://hz.chenlongwang.top/gtftabibzc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gtspecjeim.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gtygdixjiv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangkeji.top/gtawphihij.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtdrnoqxgi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tianlin.xyz/gtxmodfgpc.html

[R61] 磁盘占用
来源：http://hz.yj20258.top/gtoxbschcf.html

df -h;  du -sh *
来源：http://hz.316326.xyz/gtyjlyhnkp.html

[R62] 找最占空间的文件
来源：http://hz.xingfuxueyuan.xyz/gtkyqkjyud.html

du -ah . | sort -rh | head -10
来源：http://hz.zhaomingkeji.xyz/gtxksebtuc.html

[R63] 内存与进程
来源：http://hz.gaohongyu789.top/gtrozvhcih.html

free -h;  ps aux | grep nginx
来源：http://hz.zhixingplan.top/gtnaaevuqq.html

[R64] 结束进程
来源：http://hz.hnxiangtu.top/gtmfszfkjt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuanzhike.top/gthsrajvbk.html

[R65] 查看端口占用
来源：http://hz.jqgfzy.top/gtjqmrbbgw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yonumen.top/gtnymkiely.html

[R66] 定时任务
来源：http://hz.hywenlv.cn/gtzudmifra.html

crontab -e;  crontab -l
来源：http://hz.daria6918.cn/gtmfqkbzvp.html

[R67] 生成随机十六进制串
来源：http://hz.ybcxt.top/gtqagrleiq.html

openssl rand -hex 16
来源：http://hz.smart0.xyz/gtnaczbkwb.html

[R68] 计算文件校验值
来源：http://hz.cdnleiting.top/gtlfiqvduh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jianghu66.top/gtiirmiztw.html

[R69] 生成随机密码
来源：http://hz.vqdsnc.cn/gtkjqzyhmd.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtprfttoqt.html

[R70] 时间戳与互转
来源：http://hz.yj202588.top/gtkifjdlhy.html

date +%s;  date -d @1700000000
来源：http://hz.haohaochexian.top/gtvkpgybyj.html

[R71] 日期格式化
来源：http://hz.aizwys.cn/gtbysnncbh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hongshengwenyu.top/gtazqmkpue.html

[R72] 等待端口就绪
来源：http://hz.zhengqikj.top/gtgkcjwbzi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gtivmpyuro.html

[R73] 分割大日志
来源：http://hz.cheryme.top/gtfhntwcrh.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtbrwesgcw.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gtdvoftwie.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gtprrrcsta.html

[R75] 导出环境变量
来源：http://hz.zhongyouzk.top/gtkyxcbztb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgufenzy.top/gtxighkmdn.html

[R76] 使用临时文件
来源：http://hz.feifeiyinyue.top/gtxxvuzdmx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gttawooibd.html

[R77] 读取用户输入
来源：http://hz.sweek.top/gtxcdnxntc.html

read -rp "请输入: " ans
来源：http://hz.yj202588.top/gtqpyzgvms.html

[R78] 交互式菜单
来源：http://hz.aizwys.cn/gtekjmyigs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pengpengdd.cyou/gtsqsgbdvx.html

[R79] 解析命令行选项
来源：http://hz.ybcxt.top/gtxabvkwdl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hongshengwenyu.top/gturfjchqu.html

[R80] 查看脚本执行耗时
来源：http://hz.gzhubu.top/gtikyamhtz.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gthznjyxdy.html

================================================================================
来源：http://hz.cheryme.top/gtxptzibha.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtacnewyhe.html

================================================================================
来源：http://hz.cucudq.cn/gtrwjajeod.html

[S01] C：Hello World
来源：http://hz.vqdsnc.cn/gtoraygjsj.html

#include <stdio.h>
来源：http://hz.iojbl.cn/gtadyzghmv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xylfe.cn/gthauoyitw.html

[S02] C：变量与格式化输出
来源：http://hz.xuetiantiany.cn/gtxjuwcpyv.html

int a = 10; printf("%d\n", a);
来源：http://hz.aizwys.cn/gtvzqsrpyj.html

[S03] C：读入整数
来源：http://hz.haohaochexian.top/gtdxqcyakq.html

int x; scanf("%d", &x);
来源：http://hz.xylfe.cn/gtvyvugkwz.html

[S04] C：字符串复制
来源：http://hz.wangdashe.top/gtxsqnrdpr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.fzhhl.top/gtrnklywri.html

[S05] C：字符串长度
来源：http://hz.yanxiufei.cn/gtscgxombo.html

strlen(s)
来源：http://hz.pycfn.com/gtjulmlwqw.html

[S06] C：字符串比较
来源：http://hz.ehwqpu.com/gtjjpiplwz.html

strcmp(a, b) == 0
来源：http://hz.xinyue.icu/gttelpjogl.html

[S07] C：数组遍历求和
来源：http://hz.0kj1m.cn/gtvvlfoezr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.c1oappe.top/gttryesvtm.html

[S08] C：动态内存分配与释放
来源：http://hz.yonumen.top/gtvhrlikhl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnqzz.top/gtgybnsuzn.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtjorgzliq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.redwolf501.top/gthnnbdnkp.html

[S10] C：指针与解引用
来源：http://hz.zhiwuduotai.top/gteiyuehxw.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gtppxgllws.html

[S11] C：逐行读文件
来源：http://hz.sxryk.cn/gtyelasnqz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fzhhl.top/gtvgsygjah.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydzc1.top/gtivgkibal.html

fclose(f);
来源：http://hz.jqgufenzy.top/gtvejkmgno.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtlapswauk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.vqdsnc.cn/gtywaahzox.html

[S13] C：宏定义
来源：http://hz.c1oappe.top/gtgtzeudao.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yangfankeji.com/gthydhythd.html

[S14] C：枚举
来源：http://hz.9152youxi.cn/gtvexhvycx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.andypj.xyz/gtbkpmehjr.html

[S15] C：类型转换
来源：http://hz.daria6918.cn/gtyydpvbny.html

(double) a / b
来源：http://hz.9152youxi.cn/gtvsjmjhng.html

[S16] C：位操作置位
来源：http://hz.yangfankeji.com/gtadrepdni.html

x |= (1 << 3);
来源：http://hz.guannengcc.top/gtgekcxykp.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtvbxxxtdr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.dashuyun.cn/gtgfxvfjzn.html

[S18] C：命令行参数
来源：http://hz.zycfv.cn/gthhleawjx.html

int main(int argc, char **argv)
来源：http://hz.sufxvd.cn/gtfcsdnuua.html

[S19] C：快速排序
来源：http://hz.chenlongwang.top/gthwnhlzeq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtrnrttxxt.html

[S20] C：二分查找
来源：http://hz.dianchejie.cn/gtojdlrvzz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtgvykxhxm.html

[S21] C：字符类别判断
来源：http://hz.cdnleiting.top/gtudehoawi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xylfe.cn/gtbuscnzbm.html

[S22] C：字符串转数字
来源：http://hz.zhengqikj.top/gthbafnxat.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.mhx1999.top/gthjyttlup.html

[S23] C：随机数
来源：http://hz.yuxming.cn/gtxlarwcrm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hongshengwenyu.top/gtongoogxs.html

[S24] C：获取本地时间
来源：http://hz.shangyingyoupin.top/gtmnrvrcik.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gtnakulpgw.html

[S25] C：内存拷贝
来源：http://hz.52xcode.cn/gtliuywjax.html

memcpy(dst, src, n);
来源：http://hz.ydzc1.top/gtdpqedrhi.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtoghocsjn.html

memset(a, 0, sizeof a);
来源：http://hz.zhaomingkeji.xyz/gttaepuabn.html

[S27] C：定义常量
来源：http://hz.c1oappe.top/gtrldoxxnu.html

const double PI = 3.14159;
来源：http://hz.guannengcc.top/gtxnhqmcwf.html

[S28] C：静态变量
来源：http://hz.jyoumei.cn/gtfhbhkkfa.html

static int counter = 0;
来源：http://hz.zhiwuduotai.top/gtbllysbej.html

[S29] C：变参函数
来源：http://hz.ivvv.top/gtxcmbgokk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenzaomai.com/gttdaxmysq.html

[S30] C：头文件保护
来源：http://hz.zhaomingkeji.xyz/gtqhbcjedl.html

#ifndef X_H
来源：http://hz.cucudq.cn/gtgbpgnpib.html

#define X_H
来源：http://hz.xinyue.icu/gtwixahwpn.html

#endif
来源：http://hz.bjfxy.top/gtethajgov.html

[S31] C++：Hello World
来源：http://hz.mhx1999.top/gtjjujgjjt.html

#include <iostream>
来源：http://hz.yangfankeji.com/gtlriiijtx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenjidiqi.icu/gtharnhhrg.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtngoosqoj.html

std::string s = "hi";  s += "!";
来源：http://hz.ydjk.org.cn/gthovhtwrq.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gttpggdvhr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shzxlz.cn/gthwmobzwc.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtrnpvngxr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gtgkrpsoyb.html

[S35] C++：map
来源：http://hz.jinghuilouyu.cn/gtbmibywlp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtourxzrmi.html

[S36] C++：unordered_map
来源：http://hz.gotoacloud.top/gttlixeagb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtfmmngnuw.html

[S37] C++：set
来源：http://hz.zhongyouzk.top/gthgtkusgf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtuqstlyvl.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtbkdcxaxl.html

std::sort(v.begin(), v.end());
来源：http://hz.mhx1999.top/gtbvnzxsue.html

[S39] C++：自定义比较器排序
来源：http://hz.hywenlv.cn/gtxsbztfle.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.andypj.xyz/gtxycfghog.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtzclcfcuq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jiagoushi.top/gtxfhoxtqx.html

[S41] C++：类与构造函数
来源：http://hz.yonumen.top/gtvonsowow.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aizwys.cn/gthpziwwvt.html

[S42] C++：继承与虚函数
来源：http://hz.sufxvd.cn/gtmcmugcxq.html

class B : public Base { public: void f() override {} };
来源：http://hz.jyoumei.cn/gtptxjdsoc.html

[S43] C++：智能指针
来源：http://hz.yj20258888.top/gtjnkfteig.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydjk.org.cn/gtzgyaaqqi.html

[S44] C++：引用传参
来源：http://hz.vqdsnc.cn/gteqdhhsne.html

void inc(int &x) { ++x; }
来源：http://hz.hammf.cn/gtxwxgaaiq.html

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtouniewht.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtfxsdimop.html

[S46] C++：函数模板
来源：http://hz.svipenyu.cn/gtcawgyxvi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shuidangran.top/gtdyzljqpw.html

[S47] C++：结构化绑定遍历
来源：http://hz.jlsjyb.cn/gtujnphaml.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhaomingkeji.xyz/gtsoxxqhnv.html

[S48] C++：逐行读文件
来源：http://hz.sufxvd.cn/gtbykmejvk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtxheblwuf.html

while (std::getline(in, line)) { }
来源：http://hz.dianchejie.cn/gtmhintwec.html

[S49] C++：写文件
来源：http://hz.yj20258888.top/gtraoncsmo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hongshengwenyu.top/gtefcloeal.html

[S50] C++：格式化数字
来源：http://hz.sweek.top/gtyupkprjl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jiagoushi.top/gtqipcrncg.html

[S51] C++：显式类型转换
来源：http://hz.guowangkeji.top/gtgnwrumax.html

static_cast<double>(a) / b
来源：http://hz.wangdashe.top/gtvcxshxca.html

[S52] C++：const 与 noexcept
来源：http://hz.wangdashe.top/gtkenycexd.html

int size() const noexcept { return n_; }
来源：http://hz.mhx1999.top/gtqlhvdhsi.html

[S53] C++：移动语义
来源：http://hz.hnxiangtu.top/gtztitlmxu.html

std::vector<int> w = std::move(v);
来源：http://hz.yvedp.cn/gtuhhikgzh.html

[S54] C++：异常处理
来源：http://hz.hysaishi.cn/gthyjexwgf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xziqi.cn/gtlmkvvsgp.html

[S55] C++：结构化绑定
来源：http://hz.hfpthk.cn/gtjmwlnnwt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhiwuduotai.top/gtschpnyov.html

[S56] C++：optional
来源：http://hz.sufxvd.cn/gtrgmtjnor.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenlongwang.top/gtoabmjcae.html

[S57] C++：编译期常量
来源：http://hz.sweek.top/gtuwqrncyu.html

constexpr int N = 10;
来源：http://hz.ybcxt.top/gthyhtapoc.html

[S58] C++：命名空间
来源：http://hz.yj20258888.top/gtulwjnbsd.html

namespace ns { int f() { return 1; } }
来源：http://hz.c1oappe.top/gtltkfzeoa.html

[S59] C++：静态断言
来源：http://hz.gotoacloud.top/gtcbsnfutm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cqqwz.cn/gtmtrhabgt.html

[S60] C++：遍历并删除元素
来源：http://hz.316326.xyz/gtjxjbpjzw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydzc1.top/gtsjqsxgzj.html

================================================================================
来源：http://hz.yvedp.cn/gtqtbexnnd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtpmpvrvae.html

================================================================================
来源：http://hz.jqgufenzy.top/gttzxgfdjo.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gtgxjfdzpj.html

println("Hello")
来源：http://hz.smart0.xyz/gtppzluadm.html

[T02] Kotlin：变量
来源：http://hz.redwolf501.top/gthyxbqcmo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenlongwang.top/gtfqkkghhf.html

[T03] Kotlin：字符串模板
来源：http://hz.yj202588.top/gtlitdmrwv.html

"值: $b"
来源：http://hz.gogol.net.cn/gtwsfflovt.html

[T04] Kotlin：空安全
来源：http://hz.jianghu66.top/gtltntvqbo.html

val n: String? = null;  n?.length
来源：http://hz.xylfe.cn/gtqwxkudvx.html

[T05] Kotlin：when 表达式
来源：http://hz.andypj.xyz/gtluifqads.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ehwqpu.com/gtuytavafr.html

[T06] Kotlin：集合映射
来源：http://hz.kuanghao11.cn/gtmcvmolkz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.svipenyu.cn/gtptvwietf.html

[T07] Kotlin：集合过滤
来源：http://hz.zhixingplan.top/gtaeuddvta.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtxlptfxrv.html

[T08] Kotlin：数据类
来源：http://hz.xziqi.cn/gtbcipbvky.html

data class User(val name: String, val age: Int)
来源：http://hz.fengsongda.top/gtmugzeebh.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxuanxn.top/gtajvpizjd.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gtuructmfq.html

[T10] Kotlin：默认参数
来源：http://hz.xinyue.icu/gtogioptqw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gzhubu.top/gtpocrgfsm.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gtyostuvkp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.snrcjt.cn/gtiofaivin.html

[T12] Kotlin：解构声明
来源：http://hz.jinghuilouyu.cn/gtolfvfojl.html

val (a, b) = Pair(1, 2)
来源：http://hz.aibaodan.cn/gtgbanbyci.html

[T13] Kotlin：只读 Map
来源：http://hz.fzhhl.top/gtdevugjkh.html

val m = mapOf("a" to 1)
来源：http://hz.tianlin.xyz/gtaiobqwvy.html

[T14] Kotlin：循环
来源：http://hz.hammf.cn/gtykkelnbc.html

for (i in 1..10) println(i)
来源：http://hz.svipenyu.cn/gtackrnyrj.html

[T15] Kotlin：接口
来源：http://hz.fengsongda.top/gtkkwhgeol.html

interface Shape { fun area(): Double }
来源：http://hz.zhixingplan.top/gtnwyekqoc.html

[T16] Swift：Hello World
来源：http://hz.yongpay.top/gtiwqpnqud.html

print("Hello")
来源：http://hz.zdqjudy.top/gtzzaxrpym.html

[T17] Swift：变量与常量
来源：http://hz.jlsjyb.cn/gtxrtznivd.html

var a = 1;  let b = 2
来源：http://hz.chenzaomai.com/gthujeyeol.html

[T18] Swift：字符串插值
来源：http://hz.jyoumei.cn/gtycwmhvni.html

"值: \(b)"
来源：http://hz.nanxinkj.top/gthhnhcehi.html

[T19] Swift：可选绑定
来源：http://hz.zhaomingkeji.xyz/gtkyeiqryw.html

if let n = opt { print(n) }
来源：http://hz.ywan-chungtsiang.top/gtuaniphnu.html

[T20] Swift：数组操作
来源：http://hz.cashguo.top/gtukkarxpo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxinkj.top/gtpnejmvgx.html

[T21] Swift：遍历
来源：http://hz.gogol.net.cn/gtzvrdseun.html

for x in a { print(x) }
来源：http://hz.0kj1m.cn/gtbxtoscgc.html

[T22] Swift：字典
来源：http://hz.shangyingyoupin.top/gtdbqqfaef.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gtdgnkxrse.html

[T23] Swift：函数
来源：http://hz.zycfv.cn/gtoiodeogw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tanke756.top/gtpogddiyv.html

[T24] Swift：闭包
来源：http://hz.ydjk.org.cn/gtzppjovya.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cdnleiting.top/gtuxebiylh.html

[T25] Swift：结构体
来源：http://hz.nanxuanxn.top/gtzjwkhsbq.html

struct P { var x: Int }
来源：http://hz.ppjwa.cn/gtzjowkgup.html

[T26] Swift：类与重写
来源：http://hz.vqdsnc.cn/gtwrknywkq.html

class A: Base { override func f() {} }
来源：http://hz.xziqi.cn/gtkdbzdryu.html

[T27] Swift：错误处理
来源：http://hz.nanxinkj.top/gtkpclfywu.html

do { try f() } catch { print(error) }
来源：http://hz.guannengcc.top/gtrvwpbkof.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtobuurxao.html

enum Color { case red, green }
来源：http://hz.wangdashe.top/gthgeyanhn.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gtruviupgl.html

guard let x = opt else { return }
来源：http://hz.yj202588.top/gtgbzuwpxp.html

[T30] Swift：协议
来源：http://hz.svipenyu.cn/gtjpxempcj.html

protocol Shape { func area() -> Double }
来源：http://hz.hammf.cn/gttaodszht.html

[T31] Lua：Hello World
来源：http://hz.tianlin.xyz/gtymxqxgki.html

print("Hello")
来源：http://hz.svipenyu.cn/gtnbfhqrpo.html

[T32] Lua：局部变量
来源：http://hz.yanxiufei.cn/gtlctdzyea.html

local a = 1
来源：http://hz.jinqigufen.top/gtalitpuhg.html

[T33] Lua：表（数组）
来源：http://hz.316326.xyz/gtdblwsbmt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hfpthk.cn/gtcsvuadqw.html

[T34] Lua：遍历表
来源：http://hz.shanyushiyangtech.top/gttpncoiwa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gtvhbblver.html

[T35] Lua：字典表
来源：http://hz.yuanzhike.top/gtppykrtvd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hongshengwenyu.top/gtimuixzwo.html

[T36] Lua：函数
来源：http://hz.cashguo.top/gtbtbuwlon.html

function add(a, b) return a + b end
来源：http://hz.wangdashe.top/gthmlwsoug.html

[T37] Lua：字符串拼接
来源：http://hz.shuidangran.top/gtdgaqffjq.html

"a" .. "b"
来源：http://hz.aibaodan.cn/gtxztrcbjn.html

[T38] Lua：条件
来源：http://hz.pycfn.com/gtwiauqoon.html

if x > 0 then print("正") end
来源：http://hz.sufxvd.cn/gtjysiusby.html

[T39] Lua：模式匹配
来源：http://hz.feifeiyinyue.top/gthhrlevtz.html

string.find(s, "%d+")
来源：http://hz.birdmap.top/gtspofflla.html

[T40] Lua：元表
来源：http://hz.chenzaomai.com/gtssxbwtsi.html

setmetatable({}, { __index = base })
来源：http://hz.bjfxy.top/gthwjdxfgw.html

[T41] Perl：Hello World
来源：http://hz.pengpengdd.cyou/gtkqvpxnhc.html

print "Hello\n";
来源：http://hz.zhixingplan.top/gtprblmvna.html

[T42] Perl：变量类型
来源：http://hz.jianghu66.top/gtzwnwmelz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.pengpengdd.cyou/gtrdfibrus.html

[T43] Perl：字符串插值
来源：http://hz.yj20258888.top/gtpoeksajj.html

"值: $a"
来源：http://hz.0kj1m.cn/gturbbucrs.html

[T44] Perl：条件
来源：http://hz.jqgfzy.top/gtmrqatksx.html

if ($a > 0) { print "正"; }
来源：http://hz.shangyingyoupin.top/gtewqzgtxt.html

[T45] Perl：数组遍历
来源：http://hz.smart0.xyz/gtbhoythvt.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigfzy.top/gtwjaxdnpb.html

[T46] Perl：哈希操作
来源：http://hz.chenzaomai.com/gtieqtkduj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ivvv.top/gtntlzzuos.html


<!-- 参考信息 -->