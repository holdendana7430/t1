代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pycfn.com/gtnouwgvje.html

[R48] awk 取指定列
来源：http://hz.ydzc1.top/gtitrofldu.html

awk '{print $1, $3}' a.txt
来源：http://hz.birdmap.top/gtbcensodf.html

[R49] awk 带条件
来源：http://hz.hongshengwenyu.top/gtmrojynzd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ywan-chungtsiang.top/gtyuyvsjdu.html

[R50] awk 求和
来源：http://hz.wangshuangyany.cn/gtzqmwqxts.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtofgfapwb.html

[R51] 排序去重取前几
来源：http://hz.hammf.cn/gtnnkrqnsw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuanzhike.top/gttlgwlrpu.html

[R52] 统计行数
来源：http://hz.cheryme.top/gtljheihmw.html

wc -l a.txt
来源：http://hz.tian-w.cn/gtwrgonbzw.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gtubzgigko.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigfzy.top/gtfwjqfdtj.html

[R54] 比较两个文件
来源：http://hz.ydjk.org.cn/gtzlntxjzx.html

diff a.txt b.txt
来源：http://hz.xziqi.cn/gtllmyeyml.html

[R55] 压缩与解压
来源：http://hz.bjfxy.top/gtunsedspu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenlongwang.top/gtpnxpwdfm.html

[R56] 远程拷贝
来源：http://hz.daxiang520.top/gtjcbshvqp.html

scp file user@host:/path/
来源：http://hz.0kj1m.cn/gtebmojryx.html

[R57] 远程执行命令
来源：http://hz.9152youxi.cn/gtdyjzzzhe.html

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtacysderx.html

[R58] 下载文件
来源：http://hz.yangfankeji.com/gtnowatlba.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ppjwa.cn/gttozykxpp.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gtlczpeeuc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuanzhike.top/gtiqsaszun.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258888.top/gtzicclcas.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.svipenyu.cn/gtodedhxim.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtusyzozzi.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gtofrvhlio.html

[R62] 找最占空间的文件
来源：http://hz.guannengcc.top/gtgwuieihl.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gtrxtwnquv.html

[R63] 内存与进程
来源：http://hz.shangyingyoupin.top/gtkfocveva.html

free -h;  ps aux | grep nginx
来源：http://hz.redwolf501.top/gtkpepynhc.html

[R64] 结束进程
来源：http://hz.shuidangran.top/gtfzugmlgq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cdnleiting.top/gtushcqajf.html

[R65] 查看端口占用
来源：http://hz.aibaodan.cn/gtanuhvzrj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.birdmap.top/gtgwqlvdec.html

[R66] 定时任务
来源：http://hz.yj20258888.top/gtbnkldpua.html

crontab -e;  crontab -l
来源：http://hz.nanxuanxn.top/gtwazuatdx.html

[R67] 生成随机十六进制串
来源：http://hz.zhijiandao.cn/gtcdqrkfll.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtpunmxhlb.html

[R68] 计算文件校验值
来源：http://hz.sufxvd.cn/gtbzawlnbr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daria6918.cn/gtadfenbfn.html

[R69] 生成随机密码
来源：http://hz.yj20258.top/gtznbdstaz.html

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gtimdrssck.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtcwytqvuz.html

date +%s;  date -d @1700000000
来源：http://hz.ydjk.org.cn/gtifmkeljb.html

[R71] 日期格式化
来源：http://hz.haohaochexian.top/gtnflsrcza.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yueranfly.top/gtxagwutsh.html

[R72] 等待端口就绪
来源：http://hz.ybcxt.top/gtujkjkfkp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhijiandao.cn/gtuthphpst.html

[R73] 分割大日志
来源：http://hz.xingfuxueyuan.xyz/gtdmhzmmcu.html

split -l 1000 big.log part_
来源：http://hz.nanxinkj.top/gtysoydzje.html

[R74] 批量重命名
来源：http://hz.yueranfly.top/gtvkuvylct.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fzhhl.top/gtmvkgcjce.html

[R75] 导出环境变量
来源：http://hz.ivvv.top/gtggynnihe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenjidiqi.icu/gtriorxzgy.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtuibzaiej.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtoladhhsz.html

[R77] 读取用户输入
来源：http://hz.hongshengwenyu.top/gtjjmzjzol.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtdgtrakkv.html

[R78] 交互式菜单
来源：http://hz.tian-w.cn/gtsdhqfvov.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hongshengwenyu.top/gtmampmxrc.html

[R79] 解析命令行选项
来源：http://hz.hfpthk.cn/gtknjbweog.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gotoacloud.top/gttbzqlljq.html

[R80] 查看脚本执行耗时
来源：http://hz.haohaochexian.top/gtskqqanky.html

time ./run.sh
来源：http://hz.jinqigufen.top/gtehbkzshh.html

================================================================================
来源：http://hz.cqqwz.cn/gtbosvzmbd.html

S. C / C++ 专题
来源：http://hz.sxryk.cn/gtewdnghew.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtonfqhgsb.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtjcrbqlrg.html

#include <stdio.h>
来源：http://hz.dashuyun.cn/gtsswinwys.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zdqjudy.top/gtjfheyduk.html

[S02] C：变量与格式化输出
来源：http://hz.quarkkingdee.top/gtdjkqnusr.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtntmzplts.html

[S03] C：读入整数
来源：http://hz.yj202588.top/gtpthcprdl.html

int x; scanf("%d", &x);
来源：http://hz.zycfv.cn/gtpmcxqryt.html

[S04] C：字符串复制
来源：http://hz.cheryme.top/gtndwzfsgj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zycfv.cn/gtansthkbw.html

[S05] C：字符串长度
来源：http://hz.cashguo.top/gtwbyzkbow.html

strlen(s)
来源：http://hz.gogol.net.cn/gtwlgslhxf.html

[S06] C：字符串比较
来源：http://hz.fzhhl.top/gtpwmzvwds.html

strcmp(a, b) == 0
来源：http://hz.ehwqpu.com/gtqgabtzwt.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtdnbhjtiw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigfzy.top/gtslduuwrm.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigufen.top/gtqyqpclih.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhengqikj.top/gtuluzqxct.html

[S09] C：结构体定义与初始化
来源：http://hz.aizwys.cn/gtbqelwoej.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aizwys.cn/gtrpbeduut.html

[S10] C：指针与解引用
来源：http://hz.aibaodan.cn/gtlennfapz.html

int *p = &a;  *p = 5;
来源：http://hz.yvedp.cn/gttzbckciu.html

[S11] C：逐行读文件
来源：http://hz.zhoulong.xyz/gtdelivnzl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pycfn.com/gtvtqvesrj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangshuangyany.cn/gtcukebxxq.html

fclose(f);
来源：http://hz.quarkkingdee.top/gtlnypvfwb.html

[S12] C：写文件
来源：http://hz.chenlongwang.top/gtqyisqwpf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gtfadwpsmk.html

[S13] C：宏定义
来源：http://hz.sufxvd.cn/gtjbhrbvmw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.kuanghao11.cn/gtapjnhfpv.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtmzkptfqv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258.top/gtmjazymqj.html

[S15] C：类型转换
来源：http://hz.jlsjyb.cn/gtbbuyuuwr.html

(double) a / b
来源：http://hz.cdnleiting.top/gtnshgnuyw.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtshlsrrwh.html

x |= (1 << 3);
来源：http://hz.daria6918.cn/gtucrpmuer.html

[S17] C：安全拼接字符串
来源：http://hz.aizwys.cn/gtsxfgetbl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.feifeiyinyue.top/gtumfzjtol.html

[S18] C：命令行参数
来源：http://hz.daxiang520.top/gtsnzvzfwg.html

int main(int argc, char **argv)
来源：http://hz.zhiwuduotai.top/gtiqunqbvh.html

[S19] C：快速排序
来源：http://hz.xingfuxueyuan.xyz/gtwzpnmrxw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtdmjofckg.html

[S20] C：二分查找
来源：http://hz.316326.xyz/gtimobsjvq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gtzvhrytyr.html

[S21] C：字符类别判断
来源：http://hz.yanxiufei.cn/gtrbgoyiux.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigfzy.top/gtnsvvqfyg.html

[S22] C：字符串转数字
来源：http://hz.yangfankeji.com/gtbdtxtquv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhoulong.xyz/gtwcghlhod.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtzyyiyeav.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gtzamkeguc.html

[S24] C：获取本地时间
来源：http://hz.yangfankeji.com/gtnwxwjarv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gtpwmstjhi.html

[S25] C：内存拷贝
来源：http://hz.jinyuanbaomall.cn/gtokgwruxw.html

memcpy(dst, src, n);
来源：http://hz.cheryme.top/gttqrppylk.html

[S26] C：内存清零
来源：http://hz.havefunace.top/gtjrairvwc.html

memset(a, 0, sizeof a);
来源：http://hz.tianlin.xyz/gtmgilepny.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gthhgqosra.html

const double PI = 3.14159;
来源：http://hz.yongpay.top/gtvpvkbdbb.html

[S28] C：静态变量
来源：http://hz.c1oappe.top/gtehfupuas.html

static int counter = 0;
来源：http://hz.hammf.cn/gtxwrtekrs.html

[S29] C：变参函数
来源：http://hz.snrcjt.cn/gtvftixjky.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.haohaochexian.top/gtfcgopqgn.html

[S30] C：头文件保护
来源：http://hz.pycfn.com/gtxuezulhx.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtrbvumdab.html

#define X_H
来源：http://hz.kuanghao11.cn/gtxdcasihn.html

#endif
来源：http://hz.gzhubu.top/gtgmgjdmcs.html

[S31] C++：Hello World
来源：http://hz.meibo888.top/gtlchapqly.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtdydaedhe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtltbrpuux.html

[S32] C++：字符串
来源：http://hz.wangdashe.top/gtkwlgcwmg.html

std::string s = "hi";  s += "!";
来源：http://hz.tanke756.top/gtajgsnhpu.html

[S33] C++：vector 增删
来源：http://hz.hongshengwenyu.top/gtjdcmevaz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ywan-chungtsiang.top/gtinrueumy.html

[S34] C++：遍历 vector
来源：http://hz.316326.xyz/gtbgajvnkh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pengpengdd.cyou/gtfhqywiib.html

[S35] C++：map
来源：http://hz.xinyue.icu/gtkiqwczhi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtnrocmyvt.html

[S36] C++：unordered_map
来源：http://hz.zdqjudy.top/gtnkldvxfb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtudxquygs.html

[S37] C++：set
来源：http://hz.ydjk.org.cn/gteswlwjtr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhiwuduotai.top/gtmkhglhfl.html

[S38] C++：排序
来源：http://hz.guowangkeji.top/gtgmkgrtxy.html

std::sort(v.begin(), v.end());
来源：http://hz.ehwqpu.com/gtrjoucmds.html

[S39] C++：自定义比较器排序
来源：http://hz.9152youxi.cn/gtcjdwsqgc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.snrcjt.cn/gtoqflprmt.html

[S40] C++：查找元素
来源：http://hz.gaohongyu789.top/gtnuvregti.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yvedp.cn/gtjgrfhsqc.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gtyubrinyv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydzc1.top/gtavlzqugz.html

[S42] C++：继承与虚函数
来源：http://hz.jinqigufen.top/gtiwyknjou.html

class B : public Base { public: void f() override {} };
来源：http://hz.9152youxi.cn/gtfqpatanr.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtuyeqdpqy.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhixingplan.top/gtokkdxkzv.html

[S44] C++：引用传参
来源：http://hz.snrcjt.cn/gtcwpsqhui.html

void inc(int &x) { ++x; }
来源：http://hz.andypj.xyz/gtagytlxpn.html

[S45] C++：lambda
来源：http://hz.ivvv.top/gtamhrnywy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hnxiangtu.top/gtsfkfpzud.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gtcukzuzfp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jianghu66.top/gtqjawytbb.html

[S47] C++：结构化绑定遍历
来源：http://hz.dashuyun.cn/gtcmfgsdji.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shuidangran.top/gtnzekqhyn.html

[S48] C++：逐行读文件
来源：http://hz.shzxlz.cn/gtryjxarnn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhaomingkeji.xyz/gtkkolwtof.html

while (std::getline(in, line)) { }
来源：http://hz.jinyuanbaomall.cn/gtdsbnqcgz.html

[S49] C++：写文件
来源：http://hz.ppjwa.cn/gtrkdtlazu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj202588.top/gtaecjdnoq.html

[S50] C++：格式化数字
来源：http://hz.cheryme.top/gttxomzaau.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xinyue.icu/gtjmqprztx.html

[S51] C++：显式类型转换
来源：http://hz.cheryme.top/gtkxlepvds.html

static_cast<double>(a) / b
来源：http://hz.yuanzhike.top/gtvvytwjux.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangkeji.top/gtncftygoe.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtdlmbunct.html

[S53] C++：移动语义
来源：http://hz.jqgfzy.top/gtsjbmsubk.html

std::vector<int> w = std::move(v);
来源：http://hz.yvedp.cn/gtkpdlhtgl.html

[S54] C++：异常处理
来源：http://hz.yuxming.cn/gttfimctsn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangshuangyany.cn/gtxzcktjxl.html

[S55] C++：结构化绑定
来源：http://hz.jinqigufen.top/gtlsguwvse.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.kuanghao11.cn/gthxmgqmla.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtgjszvgwz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.haohaochexian.top/gtetqcrdun.html

[S57] C++：编译期常量
来源：http://hz.sxryk.cn/gttjixbyex.html

constexpr int N = 10;
来源：http://hz.chenzaomai.com/gttesqoarl.html

[S58] C++：命名空间
来源：http://hz.tianlin.xyz/gtjhdcwkqt.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtjyoojfaf.html

[S59] C++：静态断言
来源：http://hz.wangshuangyany.cn/gtndikzboy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gtoljqxruk.html

[S60] C++：遍历并删除元素
来源：http://hz.pycfn.com/gtpnrsiczb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xziqi.cn/gtowsvxaan.html

================================================================================
来源：http://hz.iojbl.cn/gtgbmtigxg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhijiandao.cn/gtosilqxty.html

================================================================================
来源：http://hz.chenzaomai.com/gtyivgbczi.html

[T01] Kotlin：Hello World
来源：http://hz.fengsongda.top/gtqjsijzjq.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtfcvkkuxq.html

[T02] Kotlin：变量
来源：http://hz.mhx1999.top/gtqnqxlwdd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gotoacloud.top/gtmgxpbnzc.html

[T03] Kotlin：字符串模板
来源：http://hz.smart0.xyz/gtatlvkjwm.html

"值: $b"
来源：http://hz.yvedp.cn/gtuhqguutf.html

[T04] Kotlin：空安全
来源：http://hz.tian-w.cn/gtjfxohlcw.html

val n: String? = null;  n?.length
来源：http://hz.ppjwa.cn/gtfehphzds.html

[T05] Kotlin：when 表达式
来源：http://hz.kuanghao11.cn/gtkzlhffxf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.redwolf501.top/gtnfexsqio.html

[T06] Kotlin：集合映射
来源：http://hz.xinyue.icu/gtqswupimd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgfzy.top/gtbrhesadw.html

[T07] Kotlin：集合过滤
来源：http://hz.jiagoushi.top/gtiyocthkc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.birdmap.top/gtpzebhwaq.html

[T08] Kotlin：数据类
来源：http://hz.jinqigufen.top/gtkjqxhyop.html

data class User(val name: String, val age: Int)
来源：http://hz.ppjwa.cn/gtkxotbbxv.html

[T09] Kotlin：扩展函数
来源：http://hz.yvedp.cn/gtxzyfcmag.html

fun String.exclaim() = this + "!"
来源：http://hz.shanyushiyangtech.top/gtsrqndqux.html

[T10] Kotlin：默认参数
来源：http://hz.daria6918.cn/gtaxrnhfpc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sysykeji.top/gtpvjebosa.html

[T11] Kotlin：协程
来源：http://hz.zhiwuduotai.top/gtqhqlfnql.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daxiang520.top/gthycoezcm.html

[T12] Kotlin：解构声明
来源：http://hz.daria6918.cn/gtxufrbcal.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenlongwang.top/gtjelbaqiv.html

[T13] Kotlin：只读 Map
来源：http://hz.52xcode.cn/gtciqxlwhp.html

val m = mapOf("a" to 1)
来源：http://hz.shangyingyoupin.top/gtkbvrdeqq.html

[T14] Kotlin：循环
来源：http://hz.tianlin.xyz/gtxmlyszna.html

for (i in 1..10) println(i)
来源：http://hz.quarkkingdee.top/gtonrnahao.html

[T15] Kotlin：接口
来源：http://hz.cqqwz.cn/gtfeviquao.html

interface Shape { fun area(): Double }
来源：http://hz.jyoumei.cn/gtnzigykns.html

[T16] Swift：Hello World
来源：http://hz.ydjk.org.cn/gtxovldshg.html

print("Hello")
来源：http://hz.sweek.top/gtmnuadgmg.html

[T17] Swift：变量与常量
来源：http://hz.daria6918.cn/gtmtjxpduv.html

var a = 1;  let b = 2
来源：http://hz.andypj.xyz/gtlqaawuqw.html

[T18] Swift：字符串插值
来源：http://hz.hongshengwenyu.top/gtsftvvojt.html

"值: \(b)"
来源：http://hz.iojbl.cn/gtzkmzomrc.html

[T19] Swift：可选绑定
来源：http://hz.zhengqikj.top/gtsgroqezu.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gtxxeqjfmx.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtdhvtolls.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yueranfly.top/gtbfxilvav.html

[T21] Swift：遍历
来源：http://hz.cheryme.top/gtidxghtdd.html

for x in a { print(x) }
来源：http://hz.chenzaomai.com/gtrzncyisx.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtqjvfuvni.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yuanzhike.top/gterbotfba.html

[T23] Swift：函数
来源：http://hz.dianchejie.cn/gtcxfmckzy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ivvv.top/gtxxlanpym.html

[T24] Swift：闭包
来源：http://hz.yuxming.cn/gtsbflirto.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cucudq.cn/gtkvgfkvwv.html

[T25] Swift：结构体
来源：http://hz.zycfv.cn/gtepblgxee.html

struct P { var x: Int }
来源：http://hz.nanxinkj.top/gtopxepbdy.html

[T26] Swift：类与重写
来源：http://hz.cqqwz.cn/gtmqhatsny.html

class A: Base { override func f() {} }
来源：http://hz.sxryk.cn/gtibknnibg.html

[T27] Swift：错误处理
来源：http://hz.shzxlz.cn/gtgnhbldvs.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gtlhoktkyj.html

[T28] Swift：枚举
来源：http://hz.hnxiangtu.top/gtaxdklgmf.html

enum Color { case red, green }
来源：http://hz.xinyue.icu/gteyjvnsai.html

[T29] Swift：guard 提前返回
来源：http://hz.jiagoushi.top/gtkkufbdni.html

guard let x = opt else { return }
来源：http://hz.hfpthk.cn/gtsthietru.html

[T30] Swift：协议
来源：http://hz.9152youxi.cn/gtlwcrrmtz.html

protocol Shape { func area() -> Double }
来源：http://hz.ivvv.top/gtcmrdyekx.html

[T31] Lua：Hello World
来源：http://hz.feifeiyinyue.top/gtwfecsnvw.html

print("Hello")
来源：http://hz.ehwqpu.com/gtwztvvyzd.html

[T32] Lua：局部变量
来源：http://hz.jinghuilouyu.cn/gtppiastiq.html

local a = 1
来源：http://hz.yonumen.top/gtrlilsnym.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangtech.top/gtemlbzrld.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cashguo.top/gtsyrbelbi.html

[T34] Lua：遍历表
来源：http://hz.yueranfly.top/gtzrydrqhm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xuanzx.com/gtgorpkxae.html

[T35] Lua：字典表
来源：http://hz.zhijiandao.cn/gtncgmhhdu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangshuangyany.cn/gtmjntqgdo.html

[T36] Lua：函数
来源：http://hz.ywan-chungtsiang.top/gtsxkniuob.html

function add(a, b) return a + b end
来源：http://hz.feifeiyinyue.top/gtaskzvpmj.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtrwgodpzv.html

"a" .. "b"
来源：http://hz.tianlin.xyz/gtczykqkrr.html

[T38] Lua：条件
来源：http://hz.52xcode.cn/gtfzqswzru.html

if x > 0 then print("正") end
来源：http://hz.ivvv.top/gtqakqsrkl.html

[T39] Lua：模式匹配
来源：http://hz.cqqwz.cn/gtfvzfcmdq.html

string.find(s, "%d+")
来源：http://hz.quarkkingdee.top/gteatbjnzw.html

[T40] Lua：元表
来源：http://hz.haohaochexian.top/gtloqfzioj.html

setmetatable({}, { __index = base })
来源：http://hz.sysykeji.top/gtqiyijbst.html

[T41] Perl：Hello World
来源：http://hz.zhaomingkeji.xyz/gtqfbezeqt.html

print "Hello\n";
来源：http://hz.jyoumei.cn/gtrdaohxuk.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gthodklgof.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.dianchejie.cn/gtkixqzvmv.html

[T43] Perl：字符串插值
来源：http://hz.xylfe.cn/gtdmvipetq.html

"值: $a"
来源：http://hz.sweek.top/gtxvmtdkad.html

[T44] Perl：条件
来源：http://hz.sufxvd.cn/gtldvoagyh.html

if ($a > 0) { print "正"; }
来源：http://hz.xuetiantiany.cn/gtohoeloyy.html

[T45] Perl：数组遍历
来源：http://hz.aibaodan.cn/gttxujhhel.html

for my $x (@arr) { print $x; }
来源：http://hz.ehwqpu.com/gthnkzbfyo.html

[T46] Perl：哈希操作
来源：http://hz.jqgufenzy.top/gttuaoahsg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.havefunace.top/gtybvjkfot.html

[T47] Perl：正则捕获
来源：http://hz.andypj.xyz/gtokqxevxf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sweek.top/gtctaljblu.html

[T48] Perl：正则替换
来源：http://hz.daxiang520.top/gtrgwnuazz.html

$s =~ s/old/new/g;
来源：http://hz.zhijiandao.cn/gtbsnbyufo.html

[T49] Perl：函数
来源：http://hz.gaohongyu789.top/gtiadsaaxi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.birdmap.top/gtjsldqmgi.html

[T50] Perl：逐行读文件
来源：http://hz.ydjk.org.cn/gtukxqtigz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ivvv.top/gtkuvzqnht.html


<!-- 参考信息 -->