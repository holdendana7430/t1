代发 wailian999

cmd > out.log 2>&1
来源：http://hz.guowangkeji.top/gtqihmlpjn.html

[R40] 追加写日志
来源：http://hz.zhoulong.xyz/gtwgemnisb.html

echo "log" >> out.log
来源：http://hz.nwbrower.top/gtvwptuyvh.html

[R41] 丢弃输出
来源：http://hz.havefunace.top/gtseosoeco.html

cmd >/dev/null 2>&1
来源：http://hz.shzxlz.cn/gtawbwekvc.html

[R42] 输入重定向
来源：http://hz.yongpay.top/gtatodycfv.html

wc -l < a.txt
来源：http://hz.nwbrower.top/gtazbukfxf.html

[R43] 按名字查找文件
来源：http://hz.jianghu66.top/gtrbncesxr.html

find . -name "*.log" -type f
来源：http://hz.wangshuangyany.cn/gtgwzwklxe.html

[R44] 按修改时间查找
来源：http://hz.cqqwz.cn/gtscjcbcld.html

find . -mtime -7 -type f
来源：http://hz.daria6918.cn/gtkfwyqepj.html

[R45] 批量删除
来源：http://hz.xuanzx.com/gtyaunpjgh.html

find . -name "*.tmp" -delete
来源：http://hz.zhijiandao.cn/gtexgkjqxy.html

[R46] 递归替换文件内容
来源：http://hz.gogol.net.cn/gtcklfmscu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hfpthk.cn/gtmlsgaxxn.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gtejrukltf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hongshengwenyu.top/gttypefbqp.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtxdiqftuc.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenjidiqi.icu/gtxgjxcgto.html

[R49] awk 带条件
来源：http://hz.pycfn.com/gtxkwnyied.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtumaiptgb.html

[R50] awk 求和
来源：http://hz.haohaochexian.top/gtpyheeslc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gtcgqmjtau.html

[R51] 排序去重取前几
来源：http://hz.gotoacloud.top/gtmcyxuywc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yvedp.cn/gtgslpmaai.html

[R52] 统计行数
来源：http://hz.shanyushiyangtech.top/gtngonbbnv.html

wc -l a.txt
来源：http://hz.birdmap.top/gtjwsnihxt.html

[R53] 查看文件头与实时尾
来源：http://hz.chenlongwang.top/gtnqonxhhx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aibaodan.cn/gtxahtwshe.html

[R54] 比较两个文件
来源：http://hz.yj202588.top/gtowgpxjjg.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gthonoiwtl.html

[R55] 压缩与解压
来源：http://hz.hnqzz.top/gtjirudwxv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.iojbl.cn/gtulffwvkd.html

[R56] 远程拷贝
来源：http://hz.xuetiantiany.cn/gthunyvtrl.html

scp file user@host:/path/
来源：http://hz.hfpthk.cn/gtkkjkvies.html

[R57] 远程执行命令
来源：http://hz.jyoumei.cn/gtuasmxxav.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gteqxpvwxx.html

[R58] 下载文件
来源：http://hz.c1oappe.top/gtoqjgnkpp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtbewmxsil.html

[R59] 发 POST JSON
来源：http://hz.9152youxi.cn/gtvcxlnaos.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xuanzx.com/gttvgqbzft.html

[R60] 只看 HTTP 状态码
来源：http://hz.zycfv.cn/gtohzepwep.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gtvsesoyle.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtgfscjsoe.html

df -h;  du -sh *
来源：http://hz.sxryk.cn/gthwjmtktn.html

[R62] 找最占空间的文件
来源：http://hz.ivvv.top/gtwxgazndn.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtoxpbvbxe.html

[R63] 内存与进程
来源：http://hz.zhixingplan.top/gtnxdrqeha.html

free -h;  ps aux | grep nginx
来源：http://hz.sweek.top/gtrviurubw.html

[R64] 结束进程
来源：http://hz.iojbl.cn/gtofaxhsfa.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtlbyuotfp.html

[R65] 查看端口占用
来源：http://hz.smart0.xyz/gtslowkzqa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtqkpvquoh.html

[R66] 定时任务
来源：http://hz.jinqigfzy.top/gtowxpgxie.html

crontab -e;  crontab -l
来源：http://hz.yj20258.top/gtwsagycaj.html

[R67] 生成随机十六进制串
来源：http://hz.cqqwz.cn/gtobwrseym.html

openssl rand -hex 16
来源：http://hz.wangshuangyany.cn/gtiqmnnhto.html

[R68] 计算文件校验值
来源：http://hz.ivvv.top/gtghemwkau.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jyoumei.cn/gtlzbfyiqf.html

[R69] 生成随机密码
来源：http://hz.dashuyun.cn/gttctwwluy.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtbazyuioi.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtcteipvfk.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtgvfddatg.html

[R71] 日期格式化
来源：http://hz.chenzaomai.com/gtjkmklesr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tian-w.cn/gtkarmmxmq.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gtzfusvwrt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sxryk.cn/gtazhjpnfy.html

[R73] 分割大日志
来源：http://hz.zdqjudy.top/gtjgoodspb.html

split -l 1000 big.log part_
来源：http://hz.jinqigfzy.top/gtgwkantjy.html

[R74] 批量重命名
来源：http://hz.hnxiangtu.top/gtawbyowxk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jiagoushi.top/gtyfouehpp.html

[R75] 导出环境变量
来源：http://hz.jyoumei.cn/gtbdspwylr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hysaishi.cn/gtsmteiiii.html

[R76] 使用临时文件
来源：http://hz.hnxiangtu.top/gtzjejezcj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtmlxlucse.html

[R77] 读取用户输入
来源：http://hz.hywenlv.cn/gtxkefqtyz.html

read -rp "请输入: " ans
来源：http://hz.jinqigfzy.top/gtmwqaavem.html

[R78] 交互式菜单
来源：http://hz.guowangkeji.top/gtpxqzxuvd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gotoacloud.top/gteelluvlj.html

[R79] 解析命令行选项
来源：http://hz.feifeiyinyue.top/gtoojvkmrw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guowangkeji.top/gtbgwbcvdz.html

[R80] 查看脚本执行耗时
来源：http://hz.cdnleiting.top/gtclzhntus.html

time ./run.sh
来源：http://hz.c1oappe.top/gtuoogcwrk.html

================================================================================
来源：http://hz.chenlongwang.top/gtjgfapdal.html

S. C / C++ 专题
来源：http://hz.shzxlz.cn/gtycedrqme.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtcmpfwfct.html

[S01] C：Hello World
来源：http://hz.gaohongyu789.top/gtbhukxsye.html

#include <stdio.h>
来源：http://hz.yuxming.cn/gtumzweesi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sufxvd.cn/gtlbobofhc.html

[S02] C：变量与格式化输出
来源：http://hz.zhiwuduotai.top/gtojqgvwfa.html

int a = 10; printf("%d\n", a);
来源：http://hz.meibo888.top/gtbpuscslg.html

[S03] C：读入整数
来源：http://hz.yongpay.top/gtznaiefzr.html

int x; scanf("%d", &x);
来源：http://hz.daxiang520.top/gtjjsenenn.html

[S04] C：字符串复制
来源：http://hz.xylfe.cn/gtyejeciox.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuxming.cn/gtjfhwhuug.html

[S05] C：字符串长度
来源：http://hz.cdnleiting.top/gtzefhfefw.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gttbdgsuyj.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtownrciiu.html

strcmp(a, b) == 0
来源：http://hz.sweek.top/gtanwdqyds.html

[S07] C：数组遍历求和
来源：http://hz.pycfn.com/gtnmshaqfs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guannengcc.top/gtxtoqrjdt.html

[S08] C：动态内存分配与释放
来源：http://hz.guannengcc.top/gtzfjrrwdo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangdashe.top/gtnxfazvhq.html

[S09] C：结构体定义与初始化
来源：http://hz.c1oappe.top/gtcltvpgoc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nwbrower.top/gtcfduruge.html

[S10] C：指针与解引用
来源：http://hz.nanxinkj.top/gtbvaqkpsp.html

int *p = &a;  *p = 5;
来源：http://hz.gogol.net.cn/gtzeklmhrq.html

[S11] C：逐行读文件
来源：http://hz.smart0.xyz/gtycbfnxwu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yueranfly.top/gtvqibkjap.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.mhx1999.top/gtbddnqoyu.html

fclose(f);
来源：http://hz.zdqjudy.top/gturlmzobp.html

[S12] C：写文件
来源：http://hz.guowangkeji.top/gtnkqyfumw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtjvitjlgn.html

[S13] C：宏定义
来源：http://hz.zycfv.cn/gtamdvqnaq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhiwuduotai.top/gtlqrwlrha.html

[S14] C：枚举
来源：http://hz.feifeiyinyue.top/gteazbgoby.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daxiang520.top/gtucdnamic.html

[S15] C：类型转换
来源：http://hz.iojbl.cn/gtgvddukwj.html

(double) a / b
来源：http://hz.yj202588.top/gtwvlopggx.html

[S16] C：位操作置位
来源：http://hz.nanxuanxn.top/gtbagmuakl.html

x |= (1 << 3);
来源：http://hz.dianchejie.cn/gtmvyogzjk.html

[S17] C：安全拼接字符串
来源：http://hz.tanke756.top/gtblneimdo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ehwqpu.com/gtkrpeolhk.html

[S18] C：命令行参数
来源：http://hz.nanxinkj.top/gtaoarchuz.html

int main(int argc, char **argv)
来源：http://hz.snrcjt.cn/gtzkyalram.html

[S19] C：快速排序
来源：http://hz.ydjk.org.cn/gtctmvasts.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtfgeaeevl.html

[S20] C：二分查找
来源：http://hz.yj202588.top/gttggtfdgn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtnrjptort.html

[S21] C：字符类别判断
来源：http://hz.yj20258.top/gtayyhcegh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.dianchejie.cn/gtormkikkz.html

[S22] C：字符串转数字
来源：http://hz.aizwys.cn/gthjqbifja.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cashguo.top/gtkhbchapw.html

[S23] C：随机数
来源：http://hz.sweek.top/gtthikikdi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ehwqpu.com/gtakupepjr.html

[S24] C：获取本地时间
来源：http://hz.xuanzx.com/gtdxxyokew.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yangfankeji.com/gtcdnknjeb.html

[S25] C：内存拷贝
来源：http://hz.ehwqpu.com/gtapjbvfor.html

memcpy(dst, src, n);
来源：http://hz.xuetiantiany.cn/gtlbgtpbua.html

[S26] C：内存清零
来源：http://hz.tian-w.cn/gtyzqgtazq.html

memset(a, 0, sizeof a);
来源：http://hz.ywan-chungtsiang.top/gtxtnvqbai.html

[S27] C：定义常量
来源：http://hz.xinyue.icu/gtflzodbzo.html

const double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtyykewyrh.html

[S28] C：静态变量
来源：http://hz.birdmap.top/gtcpimyhby.html

static int counter = 0;
来源：http://hz.shzxlz.cn/gtcwttwxjz.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gtcamrdsri.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj202588.top/gtvjpgsfmt.html

[S30] C：头文件保护
来源：http://hz.svipenyu.cn/gtmoskcbjv.html

#ifndef X_H
来源：http://hz.jinyuanbaomall.cn/gtefwbjcgl.html

#define X_H
来源：http://hz.gotoacloud.top/gtumgihypy.html

#endif
来源：http://hz.ybcxt.top/gtaxouxflt.html

[S31] C++：Hello World
来源：http://hz.havefunace.top/gtalncrtdb.html

#include <iostream>
来源：http://hz.chenjidiqi.icu/gtbgucswdo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.52xcode.cn/gthveqqqjf.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtgkhigfho.html

std::string s = "hi";  s += "!";
来源：http://hz.jianghu66.top/gtwwsubewx.html

[S33] C++：vector 增删
来源：http://hz.xingfuxueyuan.xyz/gtbwocbwhr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtijlbmigc.html

[S34] C++：遍历 vector
来源：http://hz.dashuyun.cn/gtnlkbshcw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yangfankeji.com/gtanmctwna.html

[S35] C++：map
来源：http://hz.jinyuanbaomall.cn/gttspjxmbd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtfhyeqyji.html

[S36] C++：unordered_map
来源：http://hz.shzxlz.cn/gtddjsrpbo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtlujngaic.html

[S37] C++：set
来源：http://hz.c1oappe.top/gteiapqiob.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xylfe.cn/gtcosydgfj.html

[S38] C++：排序
来源：http://hz.bjfxy.top/gtlmotpbie.html

std::sort(v.begin(), v.end());
来源：http://hz.jinyuanbaomall.cn/gtjezkvcqb.html

[S39] C++：自定义比较器排序
来源：http://hz.ehwqpu.com/gtocwvltim.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenlongwang.top/gtmrezvmgy.html

[S40] C++：查找元素
来源：http://hz.xziqi.cn/gtqheqcctf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cdnleiting.top/gtjonrzogz.html

[S41] C++：类与构造函数
来源：http://hz.yvedp.cn/gtstarxyrz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jiagoushi.top/gttjocbxmj.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtybwsgrqk.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtgafdmndf.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtnwczdouy.html

auto p = std::make_unique<int>(5);
来源：http://hz.sxryk.cn/gtuzbihgim.html

[S44] C++：引用传参
来源：http://hz.xziqi.cn/gtmurofoqs.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gtamedtgsr.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gtsqgptjmk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenjidiqi.icu/gtjsxqeekb.html

[S46] C++：函数模板
来源：http://hz.gaohongyu789.top/gtdhuxezkc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuanzx.com/gtdrmybihi.html

[S47] C++：结构化绑定遍历
来源：http://hz.cashguo.top/gtcwdouenz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhixingplan.top/gtgjtskkns.html

[S48] C++：逐行读文件
来源：http://hz.hysaishi.cn/gtqcbxbwwt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fzhhl.top/gtlupojstf.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtpsxxzuak.html

[S49] C++：写文件
来源：http://hz.hnqzz.top/gtpolphnbl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxinkj.top/gttbxkahtq.html

[S50] C++：格式化数字
来源：http://hz.wangdashe.top/gtfwspmxib.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuanzhike.top/gtzjksxdyn.html

[S51] C++：显式类型转换
来源：http://hz.shangyingyoupin.top/gtewqzpotq.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gtxcqvhsaq.html

[S52] C++：const 与 noexcept
来源：http://hz.havefunace.top/gtbbiyrdle.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtcjwyksxe.html

[S53] C++：移动语义
来源：http://hz.sysykeji.top/gtzmheairc.html

std::vector<int> w = std::move(v);
来源：http://hz.ybcxt.top/gtiubpzdpf.html

[S54] C++：异常处理
来源：http://hz.guowangkeji.top/gtgkvveiha.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sysykeji.top/gttjclfofz.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gtbcttetiy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yanxiufei.cn/gtfkzudafb.html

[S56] C++：optional
来源：http://hz.0kj1m.cn/gtlngqrbps.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenlongwang.top/gtcxawgfzz.html

[S57] C++：编译期常量
来源：http://hz.yanxiufei.cn/gttdpppbhr.html

constexpr int N = 10;
来源：http://hz.zhoulong.xyz/gtpszpxvpz.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtuiqkckjv.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtycccvnzy.html

[S59] C++：静态断言
来源：http://hz.zhoulong.xyz/gtmrthfzdv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangdashe.top/gtlciuygsp.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangtech.top/gtpntcdhxz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xylfe.cn/gtmjmwspvk.html

================================================================================
来源：http://hz.9152youxi.cn/gtoqnsroaq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ppjwa.cn/gtlsyirsjm.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtgkwrkhrf.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gtuowsuocr.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtbbttkpkb.html

[T02] Kotlin：变量
来源：http://hz.yvedp.cn/gtnozzxepe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gtdhjzyldj.html

[T03] Kotlin：字符串模板
来源：http://hz.jiagoushi.top/gtqkeujuag.html

"值: $b"
来源：http://hz.cashguo.top/gtlabuvyhv.html

[T04] Kotlin：空安全
来源：http://hz.haohaochexian.top/gtbvzgudkj.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtqgzxjshu.html

[T05] Kotlin：when 表达式
来源：http://hz.kuanghao11.cn/gtwcupnvli.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.316326.xyz/gtgnjzjkos.html

[T06] Kotlin：集合映射
来源：http://hz.gogol.net.cn/gtnnrngwkg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxinkj.top/gtviupbami.html

[T07] Kotlin：集合过滤
来源：http://hz.feifeiyinyue.top/gthogyifxk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ppjwa.cn/gtauasfixi.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gthzpveklv.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gtvqklpgeb.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgufenzy.top/gtipwofxqg.html

fun String.exclaim() = this + "!"
来源：http://hz.mhx1999.top/gtmtigxbqa.html

[T10] Kotlin：默认参数
来源：http://hz.jqgufenzy.top/gtooxhzfnj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhaomingkeji.xyz/gtttdvcamb.html

[T11] Kotlin：协程
来源：http://hz.ydzc1.top/gtvvabndfy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.316326.xyz/gtxsaksjja.html

[T12] Kotlin：解构声明
来源：http://hz.sxryk.cn/gtyexlyexj.html

val (a, b) = Pair(1, 2)
来源：http://hz.yueranfly.top/gttmkpkccg.html

[T13] Kotlin：只读 Map
来源：http://hz.chenzaomai.com/gtrfcwfkxj.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigfzy.top/gtfeiilddi.html

[T14] Kotlin：循环
来源：http://hz.yj20258888.top/gtlnmnizwx.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gtsgawjkaj.html

[T15] Kotlin：接口
来源：http://hz.cqqwz.cn/gtijgbavej.html

interface Shape { fun area(): Double }
来源：http://hz.tianlin.xyz/gtkjzssghi.html

[T16] Swift：Hello World
来源：http://hz.yj202588.top/gtyzdsnrga.html

print("Hello")
来源：http://hz.hnqzz.top/gtkjjvetfp.html

[T17] Swift：变量与常量
来源：http://hz.pycfn.com/gtxxoqoezt.html

var a = 1;  let b = 2
来源：http://hz.zhaomingkeji.xyz/gtfeusbavb.html

[T18] Swift：字符串插值
来源：http://hz.yangfankeji.com/gtlnscgmvg.html

"值: \(b)"
来源：http://hz.yueranfly.top/gtcebvkact.html

[T19] Swift：可选绑定
来源：http://hz.cqqwz.cn/gtrbrqryvm.html

if let n = opt { print(n) }
来源：http://hz.hywenlv.cn/gtyzcbttgf.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtkoqhpnez.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yvedp.cn/gtdiwinoah.html

[T21] Swift：遍历
来源：http://hz.ywan-chungtsiang.top/gtmqvtzitj.html

for x in a { print(x) }
来源：http://hz.haohaochexian.top/gtiixlfezx.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtqlymupgl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.redwolf501.top/gtfbetbmcy.html

[T23] Swift：函数
来源：http://hz.smart0.xyz/gtsgwkfgjl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jiagoushi.top/gtmoqgrpev.html

[T24] Swift：闭包
来源：http://hz.zhixingplan.top/gtowsfbzyr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gzhubu.top/gtizyrfrzg.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtvjunfxbx.html

struct P { var x: Int }
来源：http://hz.zhiwuduotai.top/gtznkzbenw.html

[T26] Swift：类与重写
来源：http://hz.ywan-chungtsiang.top/gtttzdfbci.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtezvbgjaz.html

[T27] Swift：错误处理
来源：http://hz.cucudq.cn/gtacuttmxr.html

do { try f() } catch { print(error) }
来源：http://hz.nanxuanxn.top/gtilobfsbh.html

[T28] Swift：枚举
来源：http://hz.zhixingplan.top/gtxmydemky.html

enum Color { case red, green }
来源：http://hz.zhaomingkeji.xyz/gtmeueigtf.html

[T29] Swift：guard 提前返回
来源：http://hz.chenzaomai.com/gtxoutmveu.html

guard let x = opt else { return }
来源：http://hz.daxiang520.top/gtnkailkoe.html

[T30] Swift：协议
来源：http://hz.yangfankeji.com/gtnuuapogd.html

protocol Shape { func area() -> Double }
来源：http://hz.xuetiantiany.cn/gtxgppnhqy.html

[T31] Lua：Hello World
来源：http://hz.hysaishi.cn/gtnzstwman.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gthdvmrjtb.html

[T32] Lua：局部变量
来源：http://hz.zhoulong.xyz/gtbodamqlt.html

local a = 1
来源：http://hz.jyoumei.cn/gthaywwiif.html

[T33] Lua：表（数组）
来源：http://hz.jinghuilouyu.cn/gtxshstpvt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yongpay.top/gtvehrmkxq.html

[T34] Lua：遍历表
来源：http://hz.shanyushiyangtech.top/gtnlypriqc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenlongwang.top/gtcheywuon.html

[T35] Lua：字典表
来源：http://hz.ydjk.org.cn/gtcjflgrva.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinyuanbaomall.cn/gttkmqjfsq.html

[T36] Lua：函数
来源：http://hz.yueranfly.top/gtntcrlgwh.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtyksbeyvr.html

[T37] Lua：字符串拼接
来源：http://hz.cdnleiting.top/gtqznpxqtq.html

"a" .. "b"
来源：http://hz.shangyingyoupin.top/gtczribwcl.html

[T38] Lua：条件
来源：http://hz.nwbrower.top/gtlllqqxls.html

if x > 0 then print("正") end
来源：http://hz.zhongyouzk.top/gtdvwixtaw.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtfmtvbwkp.html

string.find(s, "%d+")
来源：http://hz.nanxuanxn.top/gtbbicgify.html

[T40] Lua：元表
来源：http://hz.chenjidiqi.icu/gtwekvqxwu.html

setmetatable({}, { __index = base })
来源：http://hz.nanxuanxn.top/gtsbwrekee.html

[T41] Perl：Hello World
来源：http://hz.pycfn.com/gtzljsxyrw.html

print "Hello\n";
来源：http://hz.cheryme.top/gtbtvbptye.html

[T42] Perl：变量类型
来源：http://hz.bjfxy.top/gtirjtsgba.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hfpthk.cn/gtbnxcmiwf.html


<!-- 参考信息 -->