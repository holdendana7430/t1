代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtispdxpcx.html

[R36] 并发执行多个任务
来源：http://hz.zhiwuduotai.top/gtwiiskvfc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinyuanbaomall.cn/gtkzzasbww.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gtkaomyyyl.html

files=$(ls -1)
来源：http://hz.zhixingplan.top/gthbcgdmim.html

[R38] 管道串联
来源：http://hz.sysykeji.top/gtqnnzyxom.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gtufvxsetu.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtngkjrxrd.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtppsuuhix.html

[R40] 追加写日志
来源：http://hz.nwbrower.top/gtxntghpmz.html

echo "log" >> out.log
来源：http://hz.pengpengdd.cyou/gtvjngxkkj.html

[R41] 丢弃输出
来源：http://hz.sxryk.cn/gtzzslguud.html

cmd >/dev/null 2>&1
来源：http://hz.snrcjt.cn/gtcguweoes.html

[R42] 输入重定向
来源：http://hz.jlsjyb.cn/gtodocxieh.html

wc -l < a.txt
来源：http://hz.zhoulong.xyz/gtzuxftorp.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtxfobnqbi.html

find . -name "*.log" -type f
来源：http://hz.ywan-chungtsiang.top/gtmfzvnygs.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gthzspbnnp.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gtismcwsdr.html

[R45] 批量删除
来源：http://hz.52xcode.cn/gtdkhqiyrj.html

find . -name "*.tmp" -delete
来源：http://hz.hongshengwenyu.top/gtcxymeheu.html

[R46] 递归替换文件内容
来源：http://hz.dashuyun.cn/gtduhikxpk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxuanxn.top/gtotlbqqbv.html

[R47] sed 单行替换
来源：http://hz.xuanzx.com/gtvyysmvgu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gttyeqmdno.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtxuxzodqv.html

awk '{print $1, $3}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtjmvmuqgx.html

[R49] awk 带条件
来源：http://hz.pengpengdd.cyou/gtinafkzfe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtwkkafxok.html

[R50] awk 求和
来源：http://hz.redwolf501.top/gtpjvxtobc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ybcxt.top/gtpujvnilg.html

[R51] 排序去重取前几
来源：http://hz.ehwqpu.com/gtrbupzshh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yvedp.cn/gtxluyedqf.html

[R52] 统计行数
来源：http://hz.daria6918.cn/gtmztonhrf.html

wc -l a.txt
来源：http://hz.feifeiyinyue.top/gtxydclyfj.html

[R53] 查看文件头与实时尾
来源：http://hz.cqqwz.cn/gttwgoddds.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hongshengwenyu.top/gtjzdmkmic.html

[R54] 比较两个文件
来源：http://hz.fengsongda.top/gtxhpqctpe.html

diff a.txt b.txt
来源：http://hz.zdqjudy.top/gtetclawfi.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtvxqdmtlf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinghuilouyu.cn/gtxvtdbvtt.html

[R56] 远程拷贝
来源：http://hz.feifeiyinyue.top/gtugrmxgtl.html

scp file user@host:/path/
来源：http://hz.svipenyu.cn/gtfyldhffr.html

[R57] 远程执行命令
来源：http://hz.quarkkingdee.top/gtgocretbu.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtwixqgbin.html

[R58] 下载文件
来源：http://hz.0kj1m.cn/gtfjjdmsvd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.havefunace.top/gtmvpbmwhj.html

[R59] 发 POST JSON
来源：http://hz.yuanzhike.top/gtlbrecame.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hnqzz.top/gtjpgagyyc.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtbvzxkjef.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jiagoushi.top/gtubsoxnyi.html

[R61] 磁盘占用
来源：http://hz.vqdsnc.cn/gtnaqnjugo.html

df -h;  du -sh *
来源：http://hz.gogol.net.cn/gtsjjkkhze.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gttczzmxud.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtvwudheel.html

[R63] 内存与进程
来源：http://hz.shanyushiyangtech.top/gtwziruvhr.html

free -h;  ps aux | grep nginx
来源：http://hz.hnqzz.top/gtgdihykvk.html

[R64] 结束进程
来源：http://hz.andypj.xyz/gtulbtbugn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenlongwang.top/gtnpahxsxw.html

[R65] 查看端口占用
来源：http://hz.guannengcc.top/gtnwawbmzq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtvtfnmxep.html

[R66] 定时任务
来源：http://hz.jinyuanbaomall.cn/gtpsngrhgw.html

crontab -e;  crontab -l
来源：http://hz.yj20258.top/gtfatydhrz.html

[R67] 生成随机十六进制串
来源：http://hz.xylfe.cn/gtkcxkhcox.html

openssl rand -hex 16
来源：http://hz.hfpthk.cn/gtxeyjbstk.html

[R68] 计算文件校验值
来源：http://hz.fengsongda.top/gthkssflks.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zycfv.cn/gtqmpogzgl.html

[R69] 生成随机密码
来源：http://hz.tianlin.xyz/gtwiaarqox.html

head -c 16 /dev/urandom | base64
来源：http://hz.yonumen.top/gtaibuulwt.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gtdkcuzocr.html

date +%s;  date -d @1700000000
来源：http://hz.chenjidiqi.icu/gtlrrcrxpm.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtpwfsmqke.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinyuanbaomall.cn/gtkeruxkyh.html

[R72] 等待端口就绪
来源：http://hz.cdnleiting.top/gtxotrjrxc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gticiifebw.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtibqjdjeb.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtfzsqhurq.html

[R74] 批量重命名
来源：http://hz.ppjwa.cn/gtnziitcen.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cqqwz.cn/gtfzhzfjnq.html

[R75] 导出环境变量
来源：http://hz.ywan-chungtsiang.top/gtjwqwhfkv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gtngjgvzjr.html

[R76] 使用临时文件
来源：http://hz.cheryme.top/gtodumzhzn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtqbnptnda.html

[R77] 读取用户输入
来源：http://hz.xuetiantiany.cn/gtskzjycnx.html

read -rp "请输入: " ans
来源：http://hz.fzhhl.top/gtbldqlgxm.html

[R78] 交互式菜单
来源：http://hz.guowangkeji.top/gtaoeywesy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangtech.top/gthcznfiny.html

[R79] 解析命令行选项
来源：http://hz.zhoulong.xyz/gtzblzibqm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gttkzormkk.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtfsxrstka.html

time ./run.sh
来源：http://hz.pengpengdd.cyou/gtslrmpvbi.html

================================================================================
来源：http://hz.mhx1999.top/gttljtllco.html

S. C / C++ 专题
来源：http://hz.316326.xyz/gtoiwbbheh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtadbshwxy.html

[S01] C：Hello World
来源：http://hz.yueranfly.top/gtmtjmcaur.html

#include <stdio.h>
来源：http://hz.zhoulong.xyz/gtnqtxcgxe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xinyue.icu/gtdqwfgonz.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258.top/gtbpzjdjpg.html

int a = 10; printf("%d\n", a);
来源：http://hz.hongshengwenyu.top/gtsadmcgey.html

[S03] C：读入整数
来源：http://hz.wangdashe.top/gtqodbrccz.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gtyrotquaz.html

[S04] C：字符串复制
来源：http://hz.daxiang520.top/gtqwmsbtxb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.dashuyun.cn/gtghwtzngf.html

[S05] C：字符串长度
来源：http://hz.ppjwa.cn/gtbgpyhmth.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gtnqdftkvm.html

[S06] C：字符串比较
来源：http://hz.daxiang520.top/gtpunywdnr.html

strcmp(a, b) == 0
来源：http://hz.iojbl.cn/gtrhtoxkuw.html

[S07] C：数组遍历求和
来源：http://hz.yj20258.top/gtnymoogss.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cashguo.top/gtlwbtysjj.html

[S08] C：动态内存分配与释放
来源：http://hz.hongshengwenyu.top/gtikmwhfkt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhoulong.xyz/gtdbzkmxus.html

[S09] C：结构体定义与初始化
来源：http://hz.cucudq.cn/gtzrqqicbz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gotoacloud.top/gtijutetdh.html

[S10] C：指针与解引用
来源：http://hz.pengpengdd.cyou/gtqjcdudmz.html

int *p = &a;  *p = 5;
来源：http://hz.ybcxt.top/gtnrjgqpjl.html

[S11] C：逐行读文件
来源：http://hz.chenzaomai.com/gtiunityru.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinyuanbaomall.cn/gtpfjpqxrf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gthvaxukde.html

fclose(f);
来源：http://hz.chenjidiqi.icu/gtiwniuecw.html

[S12] C：写文件
来源：http://hz.zhijiandao.cn/gtcvuakhco.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yvedp.cn/gtnmhrxqyg.html

[S13] C：宏定义
来源：http://hz.gzhubu.top/gtoodldvug.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenlongwang.top/gtbcxvpvbf.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtmxyxnknu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sufxvd.cn/gtpsbaxcyb.html

[S15] C：类型转换
来源：http://hz.jinqigfzy.top/gtlyyqdnhr.html

(double) a / b
来源：http://hz.shanyushiyangtech.top/gtedyibxnt.html

[S16] C：位操作置位
来源：http://hz.xinyue.icu/gtfcfhvlby.html

x |= (1 << 3);
来源：http://hz.zhixingplan.top/gtofgsatcp.html

[S17] C：安全拼接字符串
来源：http://hz.hongshengwenyu.top/gthvvtcwgv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yueranfly.top/gtufwqcwzf.html

[S18] C：命令行参数
来源：http://hz.jiagoushi.top/gtigcusymx.html

int main(int argc, char **argv)
来源：http://hz.chenzaomai.com/gtidwwnxhp.html

[S19] C：快速排序
来源：http://hz.chenlongwang.top/gtwzoeamml.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtcovhxoqz.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtfulbgryd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtilulhube.html

[S21] C：字符类别判断
来源：http://hz.gzhubu.top/gttezfwsym.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.quarkkingdee.top/gtclzuovkg.html

[S22] C：字符串转数字
来源：http://hz.jinqigufen.top/gtiqckozqq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gotoacloud.top/gtkjibyhpx.html

[S23] C：随机数
来源：http://hz.yuanzhike.top/gtkfvuyrgz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sxryk.cn/gtutecgptk.html

[S24] C：获取本地时间
来源：http://hz.smart0.xyz/gtkuawkbru.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ivvv.top/gthlhqrwqi.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtjvxgthjo.html

memcpy(dst, src, n);
来源：http://hz.xuetiantiany.cn/gttsbclnwo.html

[S26] C：内存清零
来源：http://hz.yangfankeji.com/gtvhntsjkw.html

memset(a, 0, sizeof a);
来源：http://hz.pengpengdd.cyou/gtnjzrozde.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtthpmrgtf.html

const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtxrsdxujc.html

[S28] C：静态变量
来源：http://hz.yanxiufei.cn/gtfeczakhp.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtjfduevgz.html

[S29] C：变参函数
来源：http://hz.yj202588.top/gtnuihqvoa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hysaishi.cn/gtqjyyyhmh.html

[S30] C：头文件保护
来源：http://hz.sxryk.cn/gtticyvnmy.html

#ifndef X_H
来源：http://hz.hnxiangtu.top/gtgzheggaz.html

#define X_H
来源：http://hz.pengpengdd.cyou/gtrtbyieac.html

#endif
来源：http://hz.cqqwz.cn/gtmfbgibzj.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gtuksecncf.html

#include <iostream>
来源：http://hz.tanke756.top/gtafqbsjfo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xingfuxueyuan.xyz/gtqcrswpop.html

[S32] C++：字符串
来源：http://hz.tian-w.cn/gtrfidppka.html

std::string s = "hi";  s += "!";
来源：http://hz.yangfankeji.com/gtxcmfsknz.html

[S33] C++：vector 增删
来源：http://hz.jinghuilouyu.cn/gthnymxjhg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtndtloxbd.html

[S34] C++：遍历 vector
来源：http://hz.birdmap.top/gtuenmpjyz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ivvv.top/gtmhsstveq.html

[S35] C++：map
来源：http://hz.9152youxi.cn/gtitearvze.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtrlvllfnb.html

[S36] C++：unordered_map
来源：http://hz.cashguo.top/gtkakbdfil.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtzswqlhkp.html

[S37] C++：set
来源：http://hz.xingfuxueyuan.xyz/gtpnhiuqhb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hammf.cn/gtjyniwmma.html

[S38] C++：排序
来源：http://hz.shanyushiyangtech.top/gtpoyvarfb.html

std::sort(v.begin(), v.end());
来源：http://hz.xuetiantiany.cn/gtiuzwrval.html

[S39] C++：自定义比较器排序
来源：http://hz.cheryme.top/gtfpjwlfvt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258888.top/gtasapezwa.html

[S40] C++：查找元素
来源：http://hz.mhx1999.top/gtnwoeukrv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.9152youxi.cn/gtvzoeehnf.html

[S41] C++：类与构造函数
来源：http://hz.meibo888.top/gtxzpetfix.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.meibo888.top/gtjllgfvxx.html

[S42] C++：继承与虚函数
来源：http://hz.hammf.cn/gtgyimlfxt.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangdashe.top/gtbfhejbnu.html

[S43] C++：智能指针
来源：http://hz.jianghu66.top/gtafpiboty.html

auto p = std::make_unique<int>(5);
来源：http://hz.52xcode.cn/gtlppdcloa.html

[S44] C++：引用传参
来源：http://hz.dianchejie.cn/gtiyufydqb.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gtlepelsoi.html

[S45] C++：lambda
来源：http://hz.xingfuxueyuan.xyz/gtjrzwaggt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhengqikj.top/gtdiguyite.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gtmxdyrray.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dianchejie.cn/gtohascjzw.html

[S47] C++：结构化绑定遍历
来源：http://hz.sweek.top/gtyswpebtw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.0kj1m.cn/gtchalbxmz.html

[S48] C++：逐行读文件
来源：http://hz.yuanzhike.top/gtrugqxhln.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.kuanghao11.cn/gtrziwywyd.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtvegubiay.html

[S49] C++：写文件
来源：http://hz.ybcxt.top/gthtzkxpic.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tianlin.xyz/gtxhqsoubq.html

[S50] C++：格式化数字
来源：http://hz.hammf.cn/gtnrfdhnwv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daria6918.cn/gthdnatofg.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtgpshwcyt.html

static_cast<double>(a) / b
来源：http://hz.hnqzz.top/gtstklhtie.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtrapohjda.html

int size() const noexcept { return n_; }
来源：http://hz.jiagoushi.top/gtwfkdgtpv.html

[S53] C++：移动语义
来源：http://hz.dashuyun.cn/gtfjuulcyx.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigufen.top/gtvqcoxebq.html

[S54] C++：异常处理
来源：http://hz.kuanghao11.cn/gtjgngnkae.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jiagoushi.top/gtsjauzxdz.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtmytpmhpx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pycfn.com/gtlqbmdgdu.html

[S56] C++：optional
来源：http://hz.jlsjyb.cn/gtmufvwjuw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shuidangran.top/gtaimwggof.html

[S57] C++：编译期常量
来源：http://hz.sysykeji.top/gtsoprlmvj.html

constexpr int N = 10;
来源：http://hz.wangdashe.top/gtcvlmgcqg.html

[S58] C++：命名空间
来源：http://hz.iojbl.cn/gtgxaffyed.html

namespace ns { int f() { return 1; } }
来源：http://hz.sysykeji.top/gtszqlhvyr.html

[S59] C++：静态断言
来源：http://hz.hfpthk.cn/gtrxdbuzbd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yonumen.top/gtwofurqpe.html

[S60] C++：遍历并删除元素
来源：http://hz.shuidangran.top/gtypgsyiaj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtyctgnsbx.html

================================================================================
来源：http://hz.gogol.net.cn/gtgjetyfdt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gtqolarbbx.html

================================================================================
来源：http://hz.shzxlz.cn/gtfbawamrp.html

[T01] Kotlin：Hello World
来源：http://hz.hongshengwenyu.top/gtbbiadgky.html

println("Hello")
来源：http://hz.yangfankeji.com/gthxgvinui.html

[T02] Kotlin：变量
来源：http://hz.yongpay.top/gtxvftqzdx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenjidiqi.icu/gttljyelwy.html

[T03] Kotlin：字符串模板
来源：http://hz.hfpthk.cn/gtpkatgyjc.html

"值: $b"
来源：http://hz.cucudq.cn/gtzkwneecy.html

[T04] Kotlin：空安全
来源：http://hz.jlsjyb.cn/gtpdlftnip.html

val n: String? = null;  n?.length
来源：http://hz.nanxuanxn.top/gtuxmxthft.html

[T05] Kotlin：when 表达式
来源：http://hz.dianchejie.cn/gtkhnupxnr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.feifeiyinyue.top/gtbctdvoqy.html

[T06] Kotlin：集合映射
来源：http://hz.vqdsnc.cn/gtrxqzhnoh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hongshengwenyu.top/gtgbmspwvj.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangkeji.top/gtycloyjsw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhongyouzk.top/gtmytwfewd.html

[T08] Kotlin：数据类
来源：http://hz.mhx1999.top/gtxdhmxopp.html

data class User(val name: String, val age: Int)
来源：http://hz.cashguo.top/gtkvzrzktw.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigufen.top/gtrclfzibn.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gtmailqybr.html

[T10] Kotlin：默认参数
来源：http://hz.cheryme.top/gtdsovjtlc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.fengsongda.top/gtodepmtmr.html

[T11] Kotlin：协程
来源：http://hz.hammf.cn/gtfrpvwwti.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hysaishi.cn/gttehdymga.html

[T12] Kotlin：解构声明
来源：http://hz.c1oappe.top/gtwhpjqkvz.html

val (a, b) = Pair(1, 2)
来源：http://hz.jianghu66.top/gtmwamxlen.html

[T13] Kotlin：只读 Map
来源：http://hz.gogol.net.cn/gtvjlybvtc.html

val m = mapOf("a" to 1)
来源：http://hz.hfpthk.cn/gttyaweuuc.html

[T14] Kotlin：循环
来源：http://hz.yj20258.top/gtqhybdzyh.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtnoqtazld.html

[T15] Kotlin：接口
来源：http://hz.fzhhl.top/gtqmmitvcv.html

interface Shape { fun area(): Double }
来源：http://hz.sysykeji.top/gtizdvozpj.html

[T16] Swift：Hello World
来源：http://hz.hammf.cn/gtvsezbagu.html

print("Hello")
来源：http://hz.ydzc1.top/gtumouvhoe.html

[T17] Swift：变量与常量
来源：http://hz.cqqwz.cn/gtsybezbgo.html

var a = 1;  let b = 2
来源：http://hz.zhoulong.xyz/gtwkkwspup.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtwgebadqu.html

"值: \(b)"
来源：http://hz.birdmap.top/gtuwxmccbo.html

[T19] Swift：可选绑定
来源：http://hz.birdmap.top/gtczyqycmd.html

if let n = opt { print(n) }
来源：http://hz.zhaomingkeji.xyz/gtgtkjhtuv.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtfiiaohvz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtjwdtbwuf.html

[T21] Swift：遍历
来源：http://hz.chenjidiqi.icu/gtduotzcpi.html

for x in a { print(x) }
来源：http://hz.zhiwuduotai.top/gtvlygsqiz.html

[T22] Swift：字典
来源：http://hz.shuidangran.top/gtvbcbqyht.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.wangdashe.top/gtwqkfmsrt.html

[T23] Swift：函数
来源：http://hz.birdmap.top/gtjlzfwfkm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigufen.top/gtwsvlswss.html

[T24] Swift：闭包
来源：http://hz.sysykeji.top/gtgreulssd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinghuilouyu.cn/gtmuqjvwer.html

[T25] Swift：结构体
来源：http://hz.yongpay.top/gtzrkirftu.html

struct P { var x: Int }
来源：http://hz.jianghu66.top/gtgiqbxatr.html

[T26] Swift：类与重写
来源：http://hz.zhengqikj.top/gtbbgineda.html

class A: Base { override func f() {} }
来源：http://hz.yangfankeji.com/gtzylkajjg.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtjgnsejus.html

do { try f() } catch { print(error) }
来源：http://hz.316326.xyz/gtigwwkeeq.html

[T28] Swift：枚举
来源：http://hz.yuxming.cn/gtxprzydft.html

enum Color { case red, green }
来源：http://hz.ywan-chungtsiang.top/gtgovlwwoh.html

[T29] Swift：guard 提前返回
来源：http://hz.snrcjt.cn/gtezcmgehx.html

guard let x = opt else { return }
来源：http://hz.snrcjt.cn/gtsqcovpgf.html

[T30] Swift：协议
来源：http://hz.cashguo.top/gtlbtgzrwk.html

protocol Shape { func area() -> Double }
来源：http://hz.hywenlv.cn/gtxfepfzjc.html

[T31] Lua：Hello World
来源：http://hz.feifeiyinyue.top/gtdgkiwcpl.html

print("Hello")
来源：http://hz.fzhhl.top/gtnodgjizo.html

[T32] Lua：局部变量
来源：http://hz.hammf.cn/gtiqyvqwim.html

local a = 1
来源：http://hz.ppjwa.cn/gtzzltyldb.html

[T33] Lua：表（数组）
来源：http://hz.jinqigfzy.top/gtmsrclwtv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shanyushiyangtech.top/gtcnonvith.html

[T34] Lua：遍历表
来源：http://hz.haohaochexian.top/gtypdpjmix.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ivvv.top/gtemjqcxuj.html

[T35] Lua：字典表
来源：http://hz.chenjidiqi.icu/gtrakfyfaa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hywenlv.cn/gtsidelnnu.html

[T36] Lua：函数
来源：http://hz.chenlongwang.top/gtaexlcoin.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtzmeohghb.html

[T37] Lua：字符串拼接
来源：http://hz.vqdsnc.cn/gtrtahdlxj.html

"a" .. "b"
来源：http://hz.yuanzhike.top/gthrbjdubn.html

[T38] Lua：条件
来源：http://hz.guannengcc.top/gtkcuzkovg.html

if x > 0 then print("正") end
来源：http://hz.xingfuxueyuan.xyz/gtesuecmyd.html


<!-- 参考信息 -->