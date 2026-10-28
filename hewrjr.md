代发 wailian999

cmd >/dev/null 2>&1
来源：http://hz.chenlongwang.top/gthjyhishq.html

[R42] 输入重定向
来源：http://hz.quarkkingdee.top/gtjtyuinvn.html

wc -l < a.txt
来源：http://hz.sweek.top/gtsjanozjt.html

[R43] 按名字查找文件
来源：http://hz.yongpay.top/gtrattcbhn.html

find . -name "*.log" -type f
来源：http://hz.hammf.cn/gtdxbzrwgu.html

[R44] 按修改时间查找
来源：http://hz.shzxlz.cn/gtugpxizht.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtxtknbnxx.html

[R45] 批量删除
来源：http://hz.andypj.xyz/gtzayfjmew.html

find . -name "*.tmp" -delete
来源：http://hz.chenjidiqi.icu/gtvunnvuti.html

[R46] 递归替换文件内容
来源：http://hz.0kj1m.cn/gtcjiaqhcl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.0kj1m.cn/gtidrwhhhf.html

[R47] sed 单行替换
来源：http://hz.hysaishi.cn/gtsxsdgvjk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinqigufen.top/gtdfwzptos.html

[R48] awk 取指定列
来源：http://hz.meibo888.top/gtynnsxngy.html

awk '{print $1, $3}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtobzolkbi.html

[R49] awk 带条件
来源：http://hz.xylfe.cn/gtdoofcnxo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxinkj.top/gtvjmfnyif.html

[R50] awk 求和
来源：http://hz.tianlin.xyz/gtlxhefiik.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhengqikj.top/gtzxeklqmc.html

[R51] 排序去重取前几
来源：http://hz.yuanzhike.top/gtsiakcxfh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhongyouzk.top/gtbmhcifgi.html

[R52] 统计行数
来源：http://hz.yj202588.top/gtuszpedzy.html

wc -l a.txt
来源：http://hz.svipenyu.cn/gtqkklywge.html

[R53] 查看文件头与实时尾
来源：http://hz.kuanghao11.cn/gtsruprryo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinyuanbaomall.cn/gtrtrpksce.html

[R54] 比较两个文件
来源：http://hz.sysykeji.top/gtbujiliyn.html

diff a.txt b.txt
来源：http://hz.ywan-chungtsiang.top/gttrqjuvzh.html

[R55] 压缩与解压
来源：http://hz.yj20258.top/gtwyycunbj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guowangkeji.top/gttpxddhnu.html

[R56] 远程拷贝
来源：http://hz.yanxiufei.cn/gtzvchyllk.html

scp file user@host:/path/
来源：http://hz.yj20258.top/gtgowtnhhb.html

[R57] 远程执行命令
来源：http://hz.havefunace.top/gtwwbyopva.html

ssh user@host 'uptime'
来源：http://hz.xuetiantiany.cn/gtoevhqghj.html

[R58] 下载文件
来源：http://hz.ydzc1.top/gtayeafnay.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gotoacloud.top/gtyqnzvbqp.html

[R59] 发 POST JSON
来源：http://hz.yangfankeji.com/gtnqcmrosc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cqqwz.cn/gtevedblsy.html

[R60] 只看 HTTP 状态码
来源：http://hz.yvedp.cn/gtjmewixux.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangtech.top/gtuhdqyrfw.html

[R61] 磁盘占用
来源：http://hz.jqgfzy.top/gtewnqrzrp.html

df -h;  du -sh *
来源：http://hz.vqdsnc.cn/gtxzgmarlq.html

[R62] 找最占空间的文件
来源：http://hz.sufxvd.cn/gtdtrndhpy.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtqqnfcxmm.html

[R63] 内存与进程
来源：http://hz.jyoumei.cn/gtvvoaakxi.html

free -h;  ps aux | grep nginx
来源：http://hz.kuanghao11.cn/gtrrdxgcme.html

[R64] 结束进程
来源：http://hz.fengsongda.top/gtaubswlkv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yonumen.top/gtrzunpbnd.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtacxbztgt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yonumen.top/gtlhhsfvmd.html

[R66] 定时任务
来源：http://hz.zdqjudy.top/gthgmfugwi.html

crontab -e;  crontab -l
来源：http://hz.yvedp.cn/gtznejekju.html

[R67] 生成随机十六进制串
来源：http://hz.aizwys.cn/gtnewohazy.html

openssl rand -hex 16
来源：http://hz.hnqzz.top/gtjcfvqibv.html

[R68] 计算文件校验值
来源：http://hz.sufxvd.cn/gtzkcnwseb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtgsckaxnv.html

[R69] 生成随机密码
来源：http://hz.andypj.xyz/gtvfzeqdch.html

head -c 16 /dev/urandom | base64
来源：http://hz.316326.xyz/gtgewjlsku.html

[R70] 时间戳与互转
来源：http://hz.shangyingyoupin.top/gtcyeotutq.html

date +%s;  date -d @1700000000
来源：http://hz.c1oappe.top/gtzsucgekc.html

[R71] 日期格式化
来源：http://hz.jinyuanbaomall.cn/gtjlcmichl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhiwuduotai.top/gtzucgfvye.html

[R72] 等待端口就绪
来源：http://hz.snrcjt.cn/gtvhhjaivb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhoulong.xyz/gtifgqiytz.html

[R73] 分割大日志
来源：http://hz.ywan-chungtsiang.top/gtzbzrsvio.html

split -l 1000 big.log part_
来源：http://hz.ehwqpu.com/gtefyasihe.html

[R74] 批量重命名
来源：http://hz.jqgufenzy.top/gtnlysagpm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtumhktnht.html

[R75] 导出环境变量
来源：http://hz.nwbrower.top/gtcoaljbwn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.fzhhl.top/gtllmalvow.html

[R76] 使用临时文件
来源：http://hz.fzhhl.top/gtbryvmpyi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtbdaljngq.html

[R77] 读取用户输入
来源：http://hz.yanxiufei.cn/gtkutwgeii.html

read -rp "请输入: " ans
来源：http://hz.jianghu66.top/gtdnoccgmg.html

[R78] 交互式菜单
来源：http://hz.daxiang520.top/gtjoftpqzm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenjidiqi.icu/gttwvhwjew.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gtkcxkenwl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj202588.top/gtfbcefths.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtawrbfnph.html

time ./run.sh
来源：http://hz.quarkkingdee.top/gtsrtppnlb.html

================================================================================
来源：http://hz.pycfn.com/gtnpmwaivr.html

S. C / C++ 专题
来源：http://hz.jyoumei.cn/gtbylpapfz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtqgqvfndj.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gtyfsrdxxm.html

#include <stdio.h>
来源：http://hz.yangfankeji.com/gtpowdzgue.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhoulong.xyz/gtxoeghjaz.html

[S02] C：变量与格式化输出
来源：http://hz.kuanghao11.cn/gtgyncfvtv.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtpraegrfj.html

[S03] C：读入整数
来源：http://hz.cqqwz.cn/gtgfcnhxiu.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gtyvssbbbc.html

[S04] C：字符串复制
来源：http://hz.jqgfzy.top/gtftzvqllh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ivvv.top/gtzdgcmwgo.html

[S05] C：字符串长度
来源：http://hz.xuanzx.com/gtvedowitn.html

strlen(s)
来源：http://hz.yuanzhike.top/gtlybzcehu.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gtjhpqajqg.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtrvrfwayl.html

[S07] C：数组遍历求和
来源：http://hz.jiagoushi.top/gtanssaevp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cqqwz.cn/gtchnkldhg.html

[S08] C：动态内存分配与释放
来源：http://hz.guowangkeji.top/gtnnfjnups.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yangfankeji.com/gtoxlgcqip.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgfzy.top/gtkqrxgmex.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgfzy.top/gtcehlqodf.html

[S10] C：指针与解引用
来源：http://hz.0kj1m.cn/gtcutmgsyy.html

int *p = &a;  *p = 5;
来源：http://hz.gotoacloud.top/gtahgphahu.html

[S11] C：逐行读文件
来源：http://hz.iojbl.cn/gtjryttrpq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hfpthk.cn/gtzlgmqgko.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.316326.xyz/gtmfunqahs.html

fclose(f);
来源：http://hz.shzxlz.cn/gtvyhsaser.html

[S12] C：写文件
来源：http://hz.xuetiantiany.cn/gtiqhyfipp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhengqikj.top/gtyqstlnct.html

[S13] C：宏定义
来源：http://hz.jqgfzy.top/gtpwojknfn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhiwuduotai.top/gtftpkgqxu.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gtxomhfyfc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.birdmap.top/gtululhccu.html

[S15] C：类型转换
来源：http://hz.zhaomingkeji.xyz/gttmxzvygi.html

(double) a / b
来源：http://hz.tian-w.cn/gtswbvcisr.html

[S16] C：位操作置位
来源：http://hz.52xcode.cn/gtsodaqfqf.html

x |= (1 << 3);
来源：http://hz.chenlongwang.top/gtcbzyfbis.html

[S17] C：安全拼接字符串
来源：http://hz.birdmap.top/gtyyuanccs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtxtotvnus.html

[S18] C：命令行参数
来源：http://hz.jinqigufen.top/gtkmotnrqk.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtyykjmnwj.html

[S19] C：快速排序
来源：http://hz.9152youxi.cn/gtidgpwmiz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gtipeemiyr.html

[S20] C：二分查找
来源：http://hz.sweek.top/gtulrrjzgd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gthuhvlssp.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtnjfcdhos.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gaohongyu789.top/gttessespc.html

[S22] C：字符串转数字
来源：http://hz.0kj1m.cn/gtbvnqnibe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tanke756.top/gtfkpnelkq.html

[S23] C：随机数
来源：http://hz.52xcode.cn/gtgnrwvuzg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nwbrower.top/gtchwiytbe.html

[S24] C：获取本地时间
来源：http://hz.nanxuanxn.top/gtuzsmdtqb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxinkj.top/gtbhgicuuq.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gtxaderjdd.html

memcpy(dst, src, n);
来源：http://hz.smart0.xyz/gtuinujsxt.html

[S26] C：内存清零
来源：http://hz.ydzc1.top/gtafrrfmjy.html

memset(a, 0, sizeof a);
来源：http://hz.zhongyouzk.top/gteekphehy.html

[S27] C：定义常量
来源：http://hz.feifeiyinyue.top/gtvqcifzcf.html

const double PI = 3.14159;
来源：http://hz.sxryk.cn/gtpizkugkl.html

[S28] C：静态变量
来源：http://hz.hysaishi.cn/gtyhnazqsq.html

static int counter = 0;
来源：http://hz.yvedp.cn/gtflqxuysn.html

[S29] C：变参函数
来源：http://hz.jinqigfzy.top/gtjkxkmbcr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtxhusrqdj.html

[S30] C：头文件保护
来源：http://hz.meibo888.top/gtizlyetoa.html

#ifndef X_H
来源：http://hz.ywan-chungtsiang.top/gtmqogvhpl.html

#define X_H
来源：http://hz.yj202588.top/gtvksdjlzq.html

#endif
来源：http://hz.tianlin.xyz/gtgclkjkyg.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtqbalnvip.html

#include <iostream>
来源：http://hz.bjfxy.top/gtlrsjnhfd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cdnleiting.top/gtgnrovoed.html

[S32] C++：字符串
来源：http://hz.wangdashe.top/gtulefqlhk.html

std::string s = "hi";  s += "!";
来源：http://hz.hywenlv.cn/gthiancpvr.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangkeji.top/gtotpgnkyb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtmkpzipnv.html

[S34] C++：遍历 vector
来源：http://hz.316326.xyz/gtigcsrvrl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.quarkkingdee.top/gtvqdvarsc.html

[S35] C++：map
来源：http://hz.zdqjudy.top/gtlsvkpvla.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtfwfkxfsn.html

[S36] C++：unordered_map
来源：http://hz.jinqigfzy.top/gtesjobbsh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtynhbdmzh.html

[S37] C++：set
来源：http://hz.jinghuilouyu.cn/gtqutjmuuj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgufenzy.top/gtygyeweis.html

[S38] C++：排序
来源：http://hz.yj20258888.top/gtljtkckgo.html

std::sort(v.begin(), v.end());
来源：http://hz.zdqjudy.top/gtsffphrma.html

[S39] C++：自定义比较器排序
来源：http://hz.hysaishi.cn/gtazzwjkyx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tanke756.top/gtkdgosduo.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gtsvhzpkgr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hongshengwenyu.top/gtblxfdluj.html

[S41] C++：类与构造函数
来源：http://hz.zhengqikj.top/gtqfqyyzks.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xingfuxueyuan.xyz/gtfzqrhfji.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gtbbprlmfl.html

class B : public Base { public: void f() override {} };
来源：http://hz.jlsjyb.cn/gtnaclqzjj.html

[S43] C++：智能指针
来源：http://hz.yanxiufei.cn/gtzkeknvip.html

auto p = std::make_unique<int>(5);
来源：http://hz.jlsjyb.cn/gttdeawfqv.html

[S44] C++：引用传参
来源：http://hz.gzhubu.top/gtgnkzhybt.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigufen.top/gtujtvemdf.html

[S45] C++：lambda
来源：http://hz.daxiang520.top/gtozlrgrwn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yongpay.top/gtmzefgbiq.html

[S46] C++：函数模板
来源：http://hz.yanxiufei.cn/gtzedhzjan.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.meibo888.top/gtpiqvjmyy.html

[S47] C++：结构化绑定遍历
来源：http://hz.shzxlz.cn/gtjkjnblbz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yvedp.cn/gtoifrgljy.html

[S48] C++：逐行读文件
来源：http://hz.andypj.xyz/gtefwegmcb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhengqikj.top/gtguayywvc.html

while (std::getline(in, line)) { }
来源：http://hz.yongpay.top/gtqabovtoy.html

[S49] C++：写文件
来源：http://hz.zhixingplan.top/gtwdxlfriv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenzaomai.com/gtsracjlhy.html

[S50] C++：格式化数字
来源：http://hz.hnxiangtu.top/gtabypnxkv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shangyingyoupin.top/gtwueabzyc.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtaygmqcrw.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtgvzvwtew.html

[S52] C++：const 与 noexcept
来源：http://hz.gotoacloud.top/gtmlimwtrw.html

int size() const noexcept { return n_; }
来源：http://hz.nwbrower.top/gtvjlsgkun.html

[S53] C++：移动语义
来源：http://hz.yanxiufei.cn/gteausmttw.html

std::vector<int> w = std::move(v);
来源：http://hz.daria6918.cn/gtgdsosgxu.html

[S54] C++：异常处理
来源：http://hz.ivvv.top/gtwgsfvdpk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xylfe.cn/gtjcxmyszw.html

[S55] C++：结构化绑定
来源：http://hz.jqgufenzy.top/gttsqhgcra.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnqzz.top/gtczgptivh.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gthvjqzpfw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gtfxxlkpbn.html

[S57] C++：编译期常量
来源：http://hz.xziqi.cn/gtsbwdygya.html

constexpr int N = 10;
来源：http://hz.kuanghao11.cn/gtnvidvrzr.html

[S58] C++：命名空间
来源：http://hz.haohaochexian.top/gtnuwhlyod.html

namespace ns { int f() { return 1; } }
来源：http://hz.hywenlv.cn/gtuyxcyqjv.html

[S59] C++：静态断言
来源：http://hz.xinyue.icu/gtdbfjvruw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.birdmap.top/gtfrdiraka.html

[S60] C++：遍历并删除元素
来源：http://hz.smart0.xyz/gtevesgfbb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnqzz.top/gtlvooseaq.html

================================================================================
来源：http://hz.ppjwa.cn/gtftcnisri.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtftqhptma.html

================================================================================
来源：http://hz.ppjwa.cn/gtiahicphy.html

[T01] Kotlin：Hello World
来源：http://hz.yanxiufei.cn/gthufremmy.html

println("Hello")
来源：http://hz.gotoacloud.top/gtzxseutrl.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gtfatnbkln.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shzxlz.cn/gtyajdtzvz.html

[T03] Kotlin：字符串模板
来源：http://hz.meibo888.top/gtfqpughvh.html

"值: $b"
来源：http://hz.daria6918.cn/gtfxadulwu.html

[T04] Kotlin：空安全
来源：http://hz.chenlongwang.top/gtroawpkry.html

val n: String? = null;  n?.length
来源：http://hz.bjfxy.top/gtzljemilf.html

[T05] Kotlin：when 表达式
来源：http://hz.pengpengdd.cyou/gtvmguemmd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yonumen.top/gtaprecnei.html

[T06] Kotlin：集合映射
来源：http://hz.jiagoushi.top/gtoznrmtur.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dianchejie.cn/gthrygnbui.html

[T07] Kotlin：集合过滤
来源：http://hz.sysykeji.top/gthuhihgbi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gaohongyu789.top/gtmmepnomi.html

[T08] Kotlin：数据类
来源：http://hz.52xcode.cn/gtcpuygona.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gteojiiwpt.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgfzy.top/gtwmkftuly.html

fun String.exclaim() = this + "!"
来源：http://hz.daxiang520.top/gtxgpqvvtr.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtndikdtmn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtqdqsdhqe.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtquprfkbl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jiagoushi.top/gtcvapzdjb.html

[T12] Kotlin：解构声明
来源：http://hz.iojbl.cn/gtulzcjrtn.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydzc1.top/gtqslbivsm.html

[T13] Kotlin：只读 Map
来源：http://hz.jlsjyb.cn/gttjgvqtpt.html

val m = mapOf("a" to 1)
来源：http://hz.daxiang520.top/gtwgduoxgf.html

[T14] Kotlin：循环
来源：http://hz.yangfankeji.com/gtceyptrux.html

for (i in 1..10) println(i)
来源：http://hz.haohaochexian.top/gthdpckpvl.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gtamhrvmux.html

interface Shape { fun area(): Double }
来源：http://hz.redwolf501.top/gtcyskpact.html

[T16] Swift：Hello World
来源：http://hz.hnqzz.top/gtqnmmekjx.html

print("Hello")
来源：http://hz.shzxlz.cn/gtjsxtpgbs.html

[T17] Swift：变量与常量
来源：http://hz.hnqzz.top/gtvodtyqrd.html

var a = 1;  let b = 2
来源：http://hz.shangyingyoupin.top/gtikfhrvqk.html

[T18] Swift：字符串插值
来源：http://hz.bjfxy.top/gthagpyeuj.html

"值: \(b)"
来源：http://hz.zycfv.cn/gtestpwjxh.html

[T19] Swift：可选绑定
来源：http://hz.xylfe.cn/gtqgitvvgn.html

if let n = opt { print(n) }
来源：http://hz.yangfankeji.com/gtvoraeout.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtxsalczwn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sysykeji.top/gtprymqqln.html

[T21] Swift：遍历
来源：http://hz.hammf.cn/gtjicwwmdg.html

for x in a { print(x) }
来源：http://hz.hnqzz.top/gteputglka.html

[T22] Swift：字典
来源：http://hz.shangyingyoupin.top/gtwfvazzoz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gtqotsftos.html

[T23] Swift：函数
来源：http://hz.hywenlv.cn/gtlbytobvm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cashguo.top/gtpukhfwxt.html

[T24] Swift：闭包
来源：http://hz.daxiang520.top/gtbmftwzes.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.quarkkingdee.top/gtyngqupux.html

[T25] Swift：结构体
来源：http://hz.shuidangran.top/gthykpdovp.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtvyrwroci.html

[T26] Swift：类与重写
来源：http://hz.xuetiantiany.cn/gtkdlhifkb.html

class A: Base { override func f() {} }
来源：http://hz.zhijiandao.cn/gttksclxpf.html

[T27] Swift：错误处理
来源：http://hz.yuanzhike.top/gteblqpaqx.html

do { try f() } catch { print(error) }
来源：http://hz.kuanghao11.cn/gtnxpxsqct.html

[T28] Swift：枚举
来源：http://hz.jlsjyb.cn/gtuesqqepc.html

enum Color { case red, green }
来源：http://hz.yanxiufei.cn/gtjqykeldl.html

[T29] Swift：guard 提前返回
来源：http://hz.bjfxy.top/gtctuvpuvz.html

guard let x = opt else { return }
来源：http://hz.xinyue.icu/gtjbnbpdvt.html

[T30] Swift：协议
来源：http://hz.xinyue.icu/gtvzdhdjkx.html

protocol Shape { func area() -> Double }
来源：http://hz.yueranfly.top/gtukzhpihi.html

[T31] Lua：Hello World
来源：http://hz.guowangkeji.top/gtnerrmece.html

print("Hello")
来源：http://hz.bjfxy.top/gtxpfgncvf.html

[T32] Lua：局部变量
来源：http://hz.hysaishi.cn/gtnayxgjjl.html

local a = 1
来源：http://hz.zhiwuduotai.top/gtngjpoixf.html

[T33] Lua：表（数组）
来源：http://hz.hnqzz.top/gteutikqvy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.c1oappe.top/gtwxobbutv.html

[T34] Lua：遍历表
来源：http://hz.zhixingplan.top/gtdcjpnzql.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhongyouzk.top/gtrwwrtidj.html

[T35] Lua：字典表
来源：http://hz.guowangkeji.top/gtkbuopyvc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yonumen.top/gtqpokgfbn.html

[T36] Lua：函数
来源：http://hz.c1oappe.top/gtvljxdolj.html

function add(a, b) return a + b end
来源：http://hz.daxiang520.top/gtrvdxdhow.html

[T37] Lua：字符串拼接
来源：http://hz.jlsjyb.cn/gttjusqnmy.html

"a" .. "b"
来源：http://hz.zhixingplan.top/gtgpgruwta.html

[T38] Lua：条件
来源：http://hz.wangshuangyany.cn/gtcafsvbqf.html

if x > 0 then print("正") end
来源：http://hz.dashuyun.cn/gtcykovyxu.html

[T39] Lua：模式匹配
来源：http://hz.hnqzz.top/gthspqkxpj.html

string.find(s, "%d+")
来源：http://hz.c1oappe.top/gtivwnfbty.html

[T40] Lua：元表
来源：http://hz.ywan-chungtsiang.top/gtivcixpna.html

setmetatable({}, { __index = base })
来源：http://hz.sxryk.cn/gttoxoplta.html

[T41] Perl：Hello World
来源：http://hz.hongshengwenyu.top/gtldadpksj.html

print "Hello\n";
来源：http://hz.daria6918.cn/gtiecqvdpz.html

[T42] Perl：变量类型
来源：http://hz.jqgfzy.top/gtwfwrruob.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jlsjyb.cn/gtcncsdodw.html

[T43] Perl：字符串插值
来源：http://hz.svipenyu.cn/gtjyjqumcy.html

"值: $a"
来源：http://hz.shanyushiyangtech.top/gtdqdnuhcp.html

[T44] Perl：条件
来源：http://hz.yuanzhike.top/gteqdgorhn.html

if ($a > 0) { print "正"; }
来源：http://hz.ybcxt.top/gtjwawcuvp.html


<!-- 参考信息 -->