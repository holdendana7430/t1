代发 wailian999

cmd >/dev/null 2>&1
来源：http://hz.316326.xyz/gtzpdjcoeh.html

[R42] 输入重定向
来源：http://hz.xingfuxueyuan.xyz/gtqxlahter.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtibetvaph.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtlkrpcxcb.html

find . -name "*.log" -type f
来源：http://hz.zhijiandao.cn/gtwrngkjnb.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangkeji.top/gtvdhmkggw.html

find . -mtime -7 -type f
来源：http://hz.316326.xyz/gtwuezfygc.html

[R45] 批量删除
来源：http://hz.yuxming.cn/gtnbrprpke.html

find . -name "*.tmp" -delete
来源：http://hz.redwolf501.top/gtsyiggwql.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangkeji.top/gtjnwqnbpa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xinyue.icu/gtaqxyndhb.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gtmrqfxgvn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cheryme.top/gtnqpsihnd.html

[R48] awk 取指定列
来源：http://hz.nanxinkj.top/gtfnshohzx.html

awk '{print $1, $3}' a.txt
来源：http://hz.zdqjudy.top/gtuqozcgoh.html

[R49] awk 带条件
来源：http://hz.hywenlv.cn/gtffjzffky.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zdqjudy.top/gtbqkducqa.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtvxztxker.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.vqdsnc.cn/gtflswadzp.html

[R51] 排序去重取前几
来源：http://hz.cqqwz.cn/gtzubyxnnf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guowangkeji.top/gtxhnfecpc.html

[R52] 统计行数
来源：http://hz.ywan-chungtsiang.top/gtviqxuvxj.html

wc -l a.txt
来源：http://hz.meibo888.top/gtofewwnne.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtpcjaieod.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxinkj.top/gtkupjtiog.html

[R54] 比较两个文件
来源：http://hz.zhijiandao.cn/gtnmkvvbng.html

diff a.txt b.txt
来源：http://hz.shanyushiyangkeji.top/gtqstshowd.html

[R55] 压缩与解压
来源：http://hz.aibaodan.cn/gtpgmgwxpz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gthwgnfjun.html

[R56] 远程拷贝
来源：http://hz.ivvv.top/gtpjndysxx.html

scp file user@host:/path/
来源：http://hz.zhoulong.xyz/gtvzkhqewz.html

[R57] 远程执行命令
来源：http://hz.wangdashe.top/gtsvswbrgs.html

ssh user@host 'uptime'
来源：http://hz.mhx1999.top/gteogxoseo.html

[R58] 下载文件
来源：http://hz.cheryme.top/gtikvindxn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhijiandao.cn/gtmbvvuhjg.html

[R59] 发 POST JSON
来源：http://hz.ydzc1.top/gtssepexai.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cqqwz.cn/gtxwdhzpoh.html

[R60] 只看 HTTP 状态码
来源：http://hz.ppjwa.cn/gteenjctuf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xingfuxueyuan.xyz/gtafmamlzg.html

[R61] 磁盘占用
来源：http://hz.316326.xyz/gthvexiszn.html

df -h;  du -sh *
来源：http://hz.cheryme.top/gtnmkgkdel.html

[R62] 找最占空间的文件
来源：http://hz.zycfv.cn/gtfceacvng.html

du -ah . | sort -rh | head -10
来源：http://hz.cheryme.top/gtyurfrcxh.html

[R63] 内存与进程
来源：http://hz.yj202588.top/gtrrviefem.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgfzy.top/gtalimfhfj.html

[R64] 结束进程
来源：http://hz.yj202588.top/gtghpznbnt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gtnpuuemkn.html

[R65] 查看端口占用
来源：http://hz.ywan-chungtsiang.top/gtgjzfnsmz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jlsjyb.cn/gtwworubxk.html

[R66] 定时任务
来源：http://hz.ydjk.org.cn/gtbyutszbu.html

crontab -e;  crontab -l
来源：http://hz.hysaishi.cn/gturvgytso.html

[R67] 生成随机十六进制串
来源：http://hz.jlsjyb.cn/gtnfotxgal.html

openssl rand -hex 16
来源：http://hz.hammf.cn/gtwivupkif.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtkbejxysk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhoulong.xyz/gtbavhflyq.html

[R69] 生成随机密码
来源：http://hz.meibo888.top/gtwnetmlvp.html

head -c 16 /dev/urandom | base64
来源：http://hz.hfpthk.cn/gtugzfqasy.html

[R70] 时间戳与互转
来源：http://hz.cucudq.cn/gtyocgyfxf.html

date +%s;  date -d @1700000000
来源：http://hz.sufxvd.cn/gtouccrmnq.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtijjayout.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jyoumei.cn/gtdmruzhwp.html

[R72] 等待端口就绪
来源：http://hz.gogol.net.cn/gtmlbhcpuj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hywenlv.cn/gtiqzgrusx.html

[R73] 分割大日志
来源：http://hz.aibaodan.cn/gtqxuyhtjn.html

split -l 1000 big.log part_
来源：http://hz.dianchejie.cn/gtdelnvsbc.html

[R74] 批量重命名
来源：http://hz.zdqjudy.top/gtrvzzvrqs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenjidiqi.icu/gtnlhottge.html

[R75] 导出环境变量
来源：http://hz.xuetiantiany.cn/gttzgnrwna.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gtvmrpupam.html

[R76] 使用临时文件
来源：http://hz.shangyingyoupin.top/gtnnwigqbk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtrujjeqku.html

[R77] 读取用户输入
来源：http://hz.316326.xyz/gtlhiftybz.html

read -rp "请输入: " ans
来源：http://hz.hnxiangtu.top/gtxeswtmas.html

[R78] 交互式菜单
来源：http://hz.shangyingyoupin.top/gtonobnefl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtamyrlpqh.html

[R79] 解析命令行选项
来源：http://hz.snrcjt.cn/gtunzwbdwa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xinyue.icu/gteekkryam.html

[R80] 查看脚本执行耗时
来源：http://hz.shuidangran.top/gtvaqzwcfq.html

time ./run.sh
来源：http://hz.jinyuanbaomall.cn/gtkwbiyrgc.html

================================================================================
来源：http://hz.gotoacloud.top/gtolgfrint.html

S. C / C++ 专题
来源：http://hz.xuetiantiany.cn/gthtidxqkg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtrohudfzv.html

[S01] C：Hello World
来源：http://hz.hnqzz.top/gtcugbevla.html

#include <stdio.h>
来源：http://hz.zhijiandao.cn/gtzqaoourm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xylfe.cn/gtnsnsyegu.html

[S02] C：变量与格式化输出
来源：http://hz.ydjk.org.cn/gtgotyoseb.html

int a = 10; printf("%d\n", a);
来源：http://hz.daxiang520.top/gtmqtcgtje.html

[S03] C：读入整数
来源：http://hz.xziqi.cn/gtuaksfvfk.html

int x; scanf("%d", &x);
来源：http://hz.xylfe.cn/gtplyeevll.html

[S04] C：字符串复制
来源：http://hz.c1oappe.top/gtidhywmzj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pengpengdd.cyou/gtipmbmbck.html

[S05] C：字符串长度
来源：http://hz.jinqigufen.top/gtwqlxnlsz.html

strlen(s)
来源：http://hz.xylfe.cn/gtbqvnhqsl.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gtyfivixwg.html

strcmp(a, b) == 0
来源：http://hz.yuxming.cn/gtjxlrpwno.html

[S07] C：数组遍历求和
来源：http://hz.9152youxi.cn/gtdgzulfba.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtkrysrhjl.html

[S08] C：动态内存分配与释放
来源：http://hz.hfpthk.cn/gtbszmggqc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hfpthk.cn/gtqmgkduex.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtzhisskqc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dianchejie.cn/gttgqossdv.html

[S10] C：指针与解引用
来源：http://hz.c1oappe.top/gtcwewbaem.html

int *p = &a;  *p = 5;
来源：http://hz.birdmap.top/gtfmvbgpje.html

[S11] C：逐行读文件
来源：http://hz.xinyue.icu/gtydoertjd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sxryk.cn/gtowbsectd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ehwqpu.com/gtwaxiitaw.html

fclose(f);
来源：http://hz.jqgufenzy.top/gtwoxchwdc.html

[S12] C：写文件
来源：http://hz.sxryk.cn/gtooysmoju.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gtxixfcjdb.html

[S13] C：宏定义
来源：http://hz.hywenlv.cn/gtizyrrtte.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtvjoavfpj.html

[S14] C：枚举
来源：http://hz.fengsongda.top/gtnrrcfrfx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fzhhl.top/gtnabbxfgc.html

[S15] C：类型转换
来源：http://hz.bjfxy.top/gtrwhparop.html

(double) a / b
来源：http://hz.jianghu66.top/gtuolesnir.html

[S16] C：位操作置位
来源：http://hz.daxiang520.top/gtddcmhuhm.html

x |= (1 << 3);
来源：http://hz.ydjk.org.cn/gtfgatqorf.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gtbgobuyiv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenlongwang.top/gtgutmfago.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtevxerpvy.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtrgswztuf.html

[S19] C：快速排序
来源：http://hz.guowangkeji.top/gtlsrrrrpu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtrzhyffjj.html

[S20] C：二分查找
来源：http://hz.nanxinkj.top/gtsuojbpln.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gtyftztfiq.html

[S21] C：字符类别判断
来源：http://hz.yuanzhike.top/gtiaevxcak.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.52xcode.cn/gtmfsuymsc.html

[S22] C：字符串转数字
来源：http://hz.chenlongwang.top/gteprsfhlm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cdnleiting.top/gtbuomwikt.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtergucqfd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtovidtlfw.html

[S24] C：获取本地时间
来源：http://hz.kuanghao11.cn/gtvntgvivf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jyoumei.cn/gtgqpjiidc.html

[S25] C：内存拷贝
来源：http://hz.xziqi.cn/gtundmoebo.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtrukskmhq.html

[S26] C：内存清零
来源：http://hz.fzhhl.top/gtepzwopxo.html

memset(a, 0, sizeof a);
来源：http://hz.wangshuangyany.cn/gtyzayrqie.html

[S27] C：定义常量
来源：http://hz.zhiwuduotai.top/gtnxhxyzjz.html

const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtfgeimxok.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtprtlcauk.html

static int counter = 0;
来源：http://hz.zycfv.cn/gtqitrfpij.html

[S29] C：变参函数
来源：http://hz.hfpthk.cn/gttdgcstzd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.svipenyu.cn/gtrsmnwbsl.html

[S30] C：头文件保护
来源：http://hz.yj20258888.top/gtxfsmmnpw.html

#ifndef X_H
来源：http://hz.gogol.net.cn/gtlpbomsbe.html

#define X_H
来源：http://hz.dianchejie.cn/gtekwkfxgm.html

#endif
来源：http://hz.shanyushiyangtech.top/gtcraasnov.html

[S31] C++：Hello World
来源：http://hz.andypj.xyz/gtzkyfcdag.html

#include <iostream>
来源：http://hz.gaohongyu789.top/gtfvynunkg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cheryme.top/gtntomcrok.html

[S32] C++：字符串
来源：http://hz.zhixingplan.top/gtjxbsvozc.html

std::string s = "hi";  s += "!";
来源：http://hz.vqdsnc.cn/gtwzutrmsf.html

[S33] C++：vector 增删
来源：http://hz.cucudq.cn/gtrkgsjpkx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.316326.xyz/gtrmpmjnlp.html

[S34] C++：遍历 vector
来源：http://hz.xuetiantiany.cn/gtpvbdunqs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fengsongda.top/gtpyqppfmf.html

[S35] C++：map
来源：http://hz.yangfankeji.com/gtxtnpgvrh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtjohlkrqs.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtqjwuepcn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtijvvwsry.html

[S37] C++：set
来源：http://hz.hnxiangtu.top/gtqquettou.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuanzx.com/gtqhscvdol.html

[S38] C++：排序
来源：http://hz.chenlongwang.top/gtnwyrnhrm.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtikzwqtvv.html

[S39] C++：自定义比较器排序
来源：http://hz.fzhhl.top/gtfddyhqky.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zdqjudy.top/gtfrorpnic.html

[S40] C++：查找元素
来源：http://hz.redwolf501.top/gtzvffptku.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daxiang520.top/gtubhykamg.html

[S41] C++：类与构造函数
来源：http://hz.iojbl.cn/gtadwttsth.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cheryme.top/gtjdkgxnuy.html

[S42] C++：继承与虚函数
来源：http://hz.yanxiufei.cn/gtqtyyraeb.html

class B : public Base { public: void f() override {} };
来源：http://hz.pengpengdd.cyou/gtrfiabrit.html

[S43] C++：智能指针
来源：http://hz.smart0.xyz/gtnbeemtfb.html

auto p = std::make_unique<int>(5);
来源：http://hz.dianchejie.cn/gtqzpslpxu.html

[S44] C++：引用传参
来源：http://hz.snrcjt.cn/gtcjatqxfh.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gtsoedprks.html

[S45] C++：lambda
来源：http://hz.shangyingyoupin.top/gtxotnjqhl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.0kj1m.cn/gtirrvkddg.html

[S46] C++：函数模板
来源：http://hz.zhengqikj.top/gthlgsrhew.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtwqgcgmbw.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhoulong.xyz/gtjbosqdot.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sysykeji.top/gtaplaiizs.html

[S48] C++：逐行读文件
来源：http://hz.nanxuanxn.top/gtaxovquvm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtmvoywexr.html

while (std::getline(in, line)) { }
来源：http://hz.jlsjyb.cn/gtqfspyyjv.html

[S49] C++：写文件
来源：http://hz.jianghu66.top/gtwxrmzqhe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yvedp.cn/gtleezdlfi.html

[S50] C++：格式化数字
来源：http://hz.shanyushiyangkeji.top/gtskkmddnf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dashuyun.cn/gtznuzajmd.html

[S51] C++：显式类型转换
来源：http://hz.jinqigufen.top/gtchytiakm.html

static_cast<double>(a) / b
来源：http://hz.fzhhl.top/gtroxcgaib.html

[S52] C++：const 与 noexcept
来源：http://hz.ydjk.org.cn/gtjikwrvma.html

int size() const noexcept { return n_; }
来源：http://hz.zhongyouzk.top/gtvmzvbnet.html

[S53] C++：移动语义
来源：http://hz.hongshengwenyu.top/gtsgjapnib.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtlfxuoqyj.html

[S54] C++：异常处理
来源：http://hz.kuanghao11.cn/gtccfwtzdw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.quarkkingdee.top/gtosktttef.html

[S55] C++：结构化绑定
来源：http://hz.dianchejie.cn/gtidbaifey.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenzaomai.com/gtcctyihza.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtzueiglyk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yanxiufei.cn/gtijgrzcyh.html

[S57] C++：编译期常量
来源：http://hz.yj20258.top/gtcnzqijmp.html

constexpr int N = 10;
来源：http://hz.iojbl.cn/gtbrhulpkg.html

[S58] C++：命名空间
来源：http://hz.cqqwz.cn/gtfoybzkvv.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtqnnbhsju.html

[S59] C++：静态断言
来源：http://hz.hammf.cn/gtziozeiap.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guannengcc.top/gtlxrpmovf.html

[S60] C++：遍历并删除元素
来源：http://hz.9152youxi.cn/gtqzutyuok.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtjonxymqn.html

================================================================================
来源：http://hz.yonumen.top/gtfufaupxp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.smart0.xyz/gtkncmpzwb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzeciguus.html

[T01] Kotlin：Hello World
来源：http://hz.gotoacloud.top/gttldyymea.html

println("Hello")
来源：http://hz.hnxiangtu.top/gtmqheelzh.html

[T02] Kotlin：变量
来源：http://hz.yuanzhike.top/gtagwifhcs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.iojbl.cn/gtbmpfxbji.html

[T03] Kotlin：字符串模板
来源：http://hz.yuxming.cn/gtcdevcjpu.html

"值: $b"
来源：http://hz.zhiwuduotai.top/gtsizhclip.html

[T04] Kotlin：空安全
来源：http://hz.nwbrower.top/gtbskabjay.html

val n: String? = null;  n?.length
来源：http://hz.xingfuxueyuan.xyz/gtgwqrodnr.html

[T05] Kotlin：when 表达式
来源：http://hz.yanxiufei.cn/gtdyiuwfiz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shangyingyoupin.top/gtdyyniugr.html

[T06] Kotlin：集合映射
来源：http://hz.iojbl.cn/gtdihqifbu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxinkj.top/gthomtfpjc.html

[T07] Kotlin：集合过滤
来源：http://hz.quarkkingdee.top/gtnuizmran.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnqzz.top/gtclxmiyvi.html

[T08] Kotlin：数据类
来源：http://hz.zhongyouzk.top/gtsyqamsjz.html

data class User(val name: String, val age: Int)
来源：http://hz.nanxinkj.top/gtofsikfib.html

[T09] Kotlin：扩展函数
来源：http://hz.dianchejie.cn/gtiodggvfu.html

fun String.exclaim() = this + "!"
来源：http://hz.zhijiandao.cn/gtihzhdvwe.html

[T10] Kotlin：默认参数
来源：http://hz.feifeiyinyue.top/gtbnjiwwbf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtfnzxwgvh.html

[T11] Kotlin：协程
来源：http://hz.ybcxt.top/gtgnmkveqm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guannengcc.top/gttixnqvfm.html

[T12] Kotlin：解构声明
来源：http://hz.zycfv.cn/gtabsyljru.html

val (a, b) = Pair(1, 2)
来源：http://hz.nanxinkj.top/gtjskdnxmh.html

[T13] Kotlin：只读 Map
来源：http://hz.shzxlz.cn/gtizskmooa.html

val m = mapOf("a" to 1)
来源：http://hz.zdqjudy.top/gtymrobxaz.html

[T14] Kotlin：循环
来源：http://hz.yvedp.cn/gtqxdhwkqd.html

for (i in 1..10) println(i)
来源：http://hz.dianchejie.cn/gtcppfacql.html

[T15] Kotlin：接口
来源：http://hz.hnxiangtu.top/gtlirpttum.html

interface Shape { fun area(): Double }
来源：http://hz.xinyue.icu/gtvohaahap.html

[T16] Swift：Hello World
来源：http://hz.chenlongwang.top/gtmnejezpg.html

print("Hello")
来源：http://hz.pycfn.com/gtuoawiflv.html

[T17] Swift：变量与常量
来源：http://hz.gotoacloud.top/gtlrmtmcfz.html

var a = 1;  let b = 2
来源：http://hz.dashuyun.cn/gtcyxxapup.html

[T18] Swift：字符串插值
来源：http://hz.iojbl.cn/gtewkieyer.html

"值: \(b)"
来源：http://hz.fengsongda.top/gtgfojkcgu.html

[T19] Swift：可选绑定
来源：http://hz.chenjidiqi.icu/gtkbjmsnvq.html

if let n = opt { print(n) }
来源：http://hz.aibaodan.cn/gttccpahrd.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangtech.top/gtlghmuegr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuanzx.com/gtcbnygouj.html

[T21] Swift：遍历
来源：http://hz.chenzaomai.com/gtzldcknpr.html

for x in a { print(x) }
来源：http://hz.kuanghao11.cn/gtlsxmsyvz.html

[T22] Swift：字典
来源：http://hz.nanxuanxn.top/gtvntqzjcr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.kuanghao11.cn/gtrkkukjfh.html

[T23] Swift：函数
来源：http://hz.aibaodan.cn/gtkdedkitm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhaomingkeji.xyz/gtslrfqnuw.html

[T24] Swift：闭包
来源：http://hz.feifeiyinyue.top/gtphmckemp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj202588.top/gthrqxwful.html

[T25] Swift：结构体
来源：http://hz.9152youxi.cn/gtmwtgqzpw.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gtzowldrlm.html

[T26] Swift：类与重写
来源：http://hz.haohaochexian.top/gtmcnsnljw.html

class A: Base { override func f() {} }
来源：http://hz.daria6918.cn/gtlaoknthd.html

[T27] Swift：错误处理
来源：http://hz.yueranfly.top/gtwpngrvne.html

do { try f() } catch { print(error) }
来源：http://hz.daxiang520.top/gtlehaymqb.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtvtgepbvp.html

enum Color { case red, green }
来源：http://hz.ywan-chungtsiang.top/gthfvqgsly.html

[T29] Swift：guard 提前返回
来源：http://hz.sysykeji.top/gtaxvklnwr.html

guard let x = opt else { return }
来源：http://hz.zhengqikj.top/gtaxbzwjet.html

[T30] Swift：协议
来源：http://hz.pycfn.com/gtbovzinbz.html

protocol Shape { func area() -> Double }
来源：http://hz.jiagoushi.top/gtzxbilfku.html

[T31] Lua：Hello World
来源：http://hz.zhaomingkeji.xyz/gtjkowthpq.html

print("Hello")
来源：http://hz.jyoumei.cn/gtpocwxzri.html

[T32] Lua：局部变量
来源：http://hz.hammf.cn/gtoqyvrahg.html

local a = 1
来源：http://hz.yj20258.top/gtkhgkidip.html

[T33] Lua：表（数组）
来源：http://hz.ehwqpu.com/gtcgswvgtp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangshuangyany.cn/gtksnmttcu.html

[T34] Lua：遍历表
来源：http://hz.meibo888.top/gtykywheyb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.bjfxy.top/gtkdsgbgli.html

[T35] Lua：字典表
来源：http://hz.chenlongwang.top/gtrlljdcxq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hongshengwenyu.top/gtythxgckj.html

[T36] Lua：函数
来源：http://hz.wangdashe.top/gtkevxtvjm.html

function add(a, b) return a + b end
来源：http://hz.hywenlv.cn/gtjgrvcoiy.html

[T37] Lua：字符串拼接
来源：http://hz.yangfankeji.com/gtozrfikme.html

"a" .. "b"
来源：http://hz.mhx1999.top/gtmmzmrqmt.html

[T38] Lua：条件
来源：http://hz.snrcjt.cn/gtaykoolyl.html

if x > 0 then print("正") end
来源：http://hz.zhaomingkeji.xyz/gtabnluttr.html

[T39] Lua：模式匹配
来源：http://hz.haohaochexian.top/gtbnlvfawj.html

string.find(s, "%d+")
来源：http://hz.xinyue.icu/gtpwxfcmit.html

[T40] Lua：元表
来源：http://hz.jyoumei.cn/gtairbmnex.html

setmetatable({}, { __index = base })
来源：http://hz.zhiwuduotai.top/gtxcvoyvwy.html

[T41] Perl：Hello World
来源：http://hz.mhx1999.top/gtrixiiejr.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtqnnylcsi.html

[T42] Perl：变量类型
来源：http://hz.316326.xyz/gtztzkzrze.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jianghu66.top/gtmfjjbwjy.html

[T43] Perl：字符串插值
来源：http://hz.mhx1999.top/gtyltnzxfd.html

"值: $a"
来源：http://hz.ydzc1.top/gtrshwpyeg.html

[T44] Perl：条件
来源：http://hz.chenlongwang.top/gtvzraurls.html

if ($a > 0) { print "正"; }
来源：http://hz.xinyue.icu/gtlahfesdn.html


<!-- 参考信息 -->