代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.c1oappe.top/gtannorlht.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangkeji.top/gtcqmikkke.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jyoumei.cn/gtfiotupmp.html

[R33] 捕获错误并提示行号
来源：http://hz.jianghu66.top/gtsbztlndx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cdnleiting.top/gttqpkffaq.html

[R34] 退出时清理
来源：http://hz.yj20258.top/gtgiagkjgw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtcmhpohen.html

[R35] 后台执行并等待
来源：http://hz.snrcjt.cn/gtuwldgzqs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aizwys.cn/gtlcuqctax.html

[R36] 并发执行多个任务
来源：http://hz.jlsjyb.cn/gtdzzktqpq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cqqwz.cn/gtromntwmf.html

[R37] 把输出赋给变量
来源：http://hz.ybcxt.top/gtxhdbnpwd.html

files=$(ls -1)
来源：http://hz.meibo888.top/gtxdfglyag.html

[R38] 管道串联
来源：http://hz.hnqzz.top/gtfgknjval.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gaohongyu789.top/gtetayifqf.html

[R39] 重定向标准输出与错误
来源：http://hz.guowangkeji.top/gtcfforufc.html

cmd > out.log 2>&1
来源：http://hz.zhongyouzk.top/gtbbazwrhd.html

[R40] 追加写日志
来源：http://hz.hammf.cn/gtxygxsddi.html

echo "log" >> out.log
来源：http://hz.yonumen.top/gtpvlaaiwk.html

[R41] 丢弃输出
来源：http://hz.zhijiandao.cn/gtfmndrqsi.html

cmd >/dev/null 2>&1
来源：http://hz.iojbl.cn/gtojtmixse.html

[R42] 输入重定向
来源：http://hz.cucudq.cn/gtrtvrlwfu.html

wc -l < a.txt
来源：http://hz.chenjidiqi.icu/gtktqxwbmx.html

[R43] 按名字查找文件
来源：http://hz.ppjwa.cn/gtvckagqkc.html

find . -name "*.log" -type f
来源：http://hz.zhaomingkeji.xyz/gtocmfctul.html

[R44] 按修改时间查找
来源：http://hz.chenlongwang.top/gthcfkxmfi.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtzvhinroq.html

[R45] 批量删除
来源：http://hz.yongpay.top/gtsboaoqxp.html

find . -name "*.tmp" -delete
来源：http://hz.yanxiufei.cn/gtxxlhwvoz.html

[R46] 递归替换文件内容
来源：http://hz.9152youxi.cn/gtouaixyox.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.mhx1999.top/gtvyndspbe.html

[R47] sed 单行替换
来源：http://hz.kuanghao11.cn/gtlhaxjoln.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtixndydmo.html

[R48] awk 取指定列
来源：http://hz.hywenlv.cn/gtlsjnfrdd.html

awk '{print $1, $3}' a.txt
来源：http://hz.gaohongyu789.top/gtvpaebvjt.html

[R49] awk 带条件
来源：http://hz.zhaomingkeji.xyz/gtzhqyttjk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.havefunace.top/gtbuqluvvm.html

[R50] awk 求和
来源：http://hz.yvedp.cn/gtxcprzpse.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gzhubu.top/gtghyxjqqx.html

[R51] 排序去重取前几
来源：http://hz.xziqi.cn/gtrdvzfbbf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangdashe.top/gtgxzjwada.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtcmbedncu.html

wc -l a.txt
来源：http://hz.ydzc1.top/gtkkaalcxw.html

[R53] 查看文件头与实时尾
来源：http://hz.cqqwz.cn/gtdezppvyl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yueranfly.top/gtnznblatm.html

[R54] 比较两个文件
来源：http://hz.bjfxy.top/gteaqwehvg.html

diff a.txt b.txt
来源：http://hz.cashguo.top/gtbxsdcewy.html

[R55] 压缩与解压
来源：http://hz.gaohongyu789.top/gtccqshaxy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxinkj.top/gttqhgsgoa.html

[R56] 远程拷贝
来源：http://hz.316326.xyz/gtiwqxrwct.html

scp file user@host:/path/
来源：http://hz.jqgufenzy.top/gttbhgftbr.html

[R57] 远程执行命令
来源：http://hz.xuanzx.com/gtvxwqtyoy.html

ssh user@host 'uptime'
来源：http://hz.hammf.cn/gtmvkbhxlu.html

[R58] 下载文件
来源：http://hz.chenlongwang.top/gtlpgiwnhu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cheryme.top/gtzqazyjbx.html

[R59] 发 POST JSON
来源：http://hz.shangyingyoupin.top/gtdbjlulvm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.birdmap.top/gtqppszwdq.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenjidiqi.icu/gtvveoikij.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gtvphavdpo.html

[R61] 磁盘占用
来源：http://hz.wangshuangyany.cn/gtxmrdtckt.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtlernhwbp.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtbbvzplhn.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gtbikmrrjc.html

[R63] 内存与进程
来源：http://hz.yuanzhike.top/gtpjafdwei.html

free -h;  ps aux | grep nginx
来源：http://hz.jiagoushi.top/gtmusuiwxs.html

[R64] 结束进程
来源：http://hz.hnxiangtu.top/gtaejdocsg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tanke756.top/gtueuxhgjs.html

[R65] 查看端口占用
来源：http://hz.hywenlv.cn/gtiluofmtt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtgivktkie.html

[R66] 定时任务
来源：http://hz.chenjidiqi.icu/gtbmiebxmm.html

crontab -e;  crontab -l
来源：http://hz.cdnleiting.top/gtagvbzjqz.html

[R67] 生成随机十六进制串
来源：http://hz.cashguo.top/gtviosrihq.html

openssl rand -hex 16
来源：http://hz.yuanzhike.top/gtnxjcmaiw.html

[R68] 计算文件校验值
来源：http://hz.52xcode.cn/gtfetpgixa.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aibaodan.cn/gtdgmyvmik.html

[R69] 生成随机密码
来源：http://hz.chenzaomai.com/gtnkiojitu.html

head -c 16 /dev/urandom | base64
来源：http://hz.havefunace.top/gtnerleltd.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gtdluzrodu.html

date +%s;  date -d @1700000000
来源：http://hz.pengpengdd.cyou/gtroqmkqyx.html

[R71] 日期格式化
来源：http://hz.ydjk.org.cn/gttxueervo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tianlin.xyz/gtirxocppo.html

[R72] 等待端口就绪
来源：http://hz.9152youxi.cn/gtrwlobvch.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hfpthk.cn/gtykakoohw.html

[R73] 分割大日志
来源：http://hz.ywan-chungtsiang.top/gtlimvfcbm.html

split -l 1000 big.log part_
来源：http://hz.hnqzz.top/gttirebjnd.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtfhdrrcgp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.snrcjt.cn/gtdikljlay.html

[R75] 导出环境变量
来源：http://hz.nanxuanxn.top/gtpvxjlffl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sufxvd.cn/gtvirkitwl.html

[R76] 使用临时文件
来源：http://hz.jinqigfzy.top/gtshffgxzn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtdiqagrpl.html

[R77] 读取用户输入
来源：http://hz.c1oappe.top/gtgxkopqsm.html

read -rp "请输入: " ans
来源：http://hz.yanxiufei.cn/gtebpvheft.html

[R78] 交互式菜单
来源：http://hz.jinqigufen.top/gtcozqnadb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hfpthk.cn/gtfnqorhbq.html

[R79] 解析命令行选项
来源：http://hz.shangyingyoupin.top/gtjovgoyes.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gzhubu.top/gtwehycjdw.html

[R80] 查看脚本执行耗时
来源：http://hz.cheryme.top/gtzjtvsqgz.html

time ./run.sh
来源：http://hz.yuanzhike.top/gtokupwvgd.html

================================================================================
来源：http://hz.smart0.xyz/gtqxtznscg.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtbpuomskf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtidsteitm.html

[S01] C：Hello World
来源：http://hz.yj202588.top/gtykwspdfb.html

#include <stdio.h>
来源：http://hz.haohaochexian.top/gtobyhgncs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hysaishi.cn/gtxpctoaug.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gtnzgkxsmc.html

int a = 10; printf("%d\n", a);
来源：http://hz.kuanghao11.cn/gtzfuxknuw.html

[S03] C：读入整数
来源：http://hz.yangfankeji.com/gtbtkubbly.html

int x; scanf("%d", &x);
来源：http://hz.quarkkingdee.top/gtxsbmbgmj.html

[S04] C：字符串复制
来源：http://hz.wangshuangyany.cn/gtpzygwmye.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jyoumei.cn/gtaomrbcqh.html

[S05] C：字符串长度
来源：http://hz.sysykeji.top/gtkwsuyqjx.html

strlen(s)
来源：http://hz.sysykeji.top/gtutksrtgj.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gtqtppjayc.html

strcmp(a, b) == 0
来源：http://hz.jyoumei.cn/gtwxqcbohq.html

[S07] C：数组遍历求和
来源：http://hz.zhengqikj.top/gtkoeriwdk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.mhx1999.top/gtqezdfelr.html

[S08] C：动态内存分配与释放
来源：http://hz.chenjidiqi.icu/gtwhciqeel.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aizwys.cn/gtslcegouz.html

[S09] C：结构体定义与初始化
来源：http://hz.wangdashe.top/gtldvddccy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhoulong.xyz/gtrvlzfmac.html

[S10] C：指针与解引用
来源：http://hz.shzxlz.cn/gtjfbuipwe.html

int *p = &a;  *p = 5;
来源：http://hz.zdqjudy.top/gtzdzkndlm.html

[S11] C：逐行读文件
来源：http://hz.316326.xyz/gtnmvnbast.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhengqikj.top/gtgepnwozo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sysykeji.top/gtwbogmipu.html

fclose(f);
来源：http://hz.aizwys.cn/gtmzbphksm.html

[S12] C：写文件
来源：http://hz.nanxinkj.top/gtznidhzgx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ivvv.top/gtaygxnicv.html

[S13] C：宏定义
来源：http://hz.hnqzz.top/gtdqsrujhq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sweek.top/gtisrkdmts.html

[S14] C：枚举
来源：http://hz.sweek.top/gtaphsogvi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtmwffyvcw.html

[S15] C：类型转换
来源：http://hz.jqgufenzy.top/gtoyslhcwy.html

(double) a / b
来源：http://hz.feifeiyinyue.top/gttyoujxtk.html

[S16] C：位操作置位
来源：http://hz.gogol.net.cn/gtiezmpkzo.html

x |= (1 << 3);
来源：http://hz.jianghu66.top/gtcdoyvfpd.html

[S17] C：安全拼接字符串
来源：http://hz.yueranfly.top/gtssofaaaa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ywan-chungtsiang.top/gtxevvhdse.html

[S18] C：命令行参数
来源：http://hz.zycfv.cn/gthofjkcls.html

int main(int argc, char **argv)
来源：http://hz.yanxiufei.cn/gtgohntfuz.html

[S19] C：快速排序
来源：http://hz.gotoacloud.top/gtkzeydufl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtsmdiqwtk.html

[S20] C：二分查找
来源：http://hz.birdmap.top/gtwgykuowq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtncjqnimq.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gtxrmkvfsf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daxiang520.top/gtxntfhsca.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtelyaywci.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gtuhweichz.html

[S23] C：随机数
来源：http://hz.cheryme.top/gtdehcdfxh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.svipenyu.cn/gtslqyijlh.html

[S24] C：获取本地时间
来源：http://hz.quarkkingdee.top/gtluseavmf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.vqdsnc.cn/gtoadcgbdy.html

[S25] C：内存拷贝
来源：http://hz.zdqjudy.top/gtvpawrepk.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtjqlgtipv.html

[S26] C：内存清零
来源：http://hz.hysaishi.cn/gtkmbdafta.html

memset(a, 0, sizeof a);
来源：http://hz.pengpengdd.cyou/gtrcfacgna.html

[S27] C：定义常量
来源：http://hz.0kj1m.cn/gtlbqznrcn.html

const double PI = 3.14159;
来源：http://hz.meibo888.top/gturqscsyi.html

[S28] C：静态变量
来源：http://hz.fzhhl.top/gtdoiputyj.html

static int counter = 0;
来源：http://hz.havefunace.top/gtmctizfhb.html

[S29] C：变参函数
来源：http://hz.jianghu66.top/gtosuvluis.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhaomingkeji.xyz/gtynaehich.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtsxzqovof.html

#ifndef X_H
来源：http://hz.shangyingyoupin.top/gtycrxhuki.html

#define X_H
来源：http://hz.ydjk.org.cn/gtejsfnsxx.html

#endif
来源：http://hz.andypj.xyz/gtnhkmmjpx.html

[S31] C++：Hello World
来源：http://hz.shzxlz.cn/gtpessyzua.html

#include <iostream>
来源：http://hz.tanke756.top/gtwgtncivp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yanxiufei.cn/gtsrbayeku.html

[S32] C++：字符串
来源：http://hz.ybcxt.top/gtjphtaufb.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtnkhggnub.html

[S33] C++：vector 增删
来源：http://hz.shangyingyoupin.top/gtpminbqsp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258888.top/gtzeipiqcl.html

[S34] C++：遍历 vector
来源：http://hz.xinyue.icu/gtqgympjqh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtfmguszcz.html

[S35] C++：map
来源：http://hz.daria6918.cn/gtkkqwogaj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnxiangtu.top/gtvitrpkzg.html

[S36] C++：unordered_map
来源：http://hz.jlsjyb.cn/gtrypcembc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtsymkfgyu.html

[S37] C++：set
来源：http://hz.daxiang520.top/gtnufehiys.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtoivhnczx.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtkfjfvcgd.html

std::sort(v.begin(), v.end());
来源：http://hz.jiagoushi.top/gtscfrpysh.html

[S39] C++：自定义比较器排序
来源：http://hz.xuanzx.com/gtdclgpnea.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yueranfly.top/gttjkjhiak.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtjxiwqipp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.birdmap.top/gtzlnlkdyd.html

[S41] C++：类与构造函数
来源：http://hz.fzhhl.top/gtmoccsrbg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhengqikj.top/gtelevucln.html

[S42] C++：继承与虚函数
来源：http://hz.yueranfly.top/gtaxuphgzb.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenlongwang.top/gttkztbkwv.html

[S43] C++：智能指针
来源：http://hz.dashuyun.cn/gtantbxwbx.html

auto p = std::make_unique<int>(5);
来源：http://hz.52xcode.cn/gtwblenhbn.html

[S44] C++：引用传参
来源：http://hz.shzxlz.cn/gtguceyiug.html

void inc(int &x) { ++x; }
来源：http://hz.ywan-chungtsiang.top/gtkshnpjvb.html

[S45] C++：lambda
来源：http://hz.xziqi.cn/gtbvivcypg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuanzhike.top/gtytkytzoj.html

[S46] C++：函数模板
来源：http://hz.316326.xyz/gtgpdrxfky.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cqqwz.cn/gteximfwit.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtlhwjdzhn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sxryk.cn/gtrqxekael.html

[S48] C++：逐行读文件
来源：http://hz.hnxiangtu.top/gtstjptejq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cheryme.top/gtczwygdio.html

while (std::getline(in, line)) { }
来源：http://hz.kuanghao11.cn/gthindqwof.html

[S49] C++：写文件
来源：http://hz.hammf.cn/gtaadtagpz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cheryme.top/gtigpbzkyj.html

[S50] C++：格式化数字
来源：http://hz.hywenlv.cn/gtyqqvefcg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gttajguzgz.html

[S51] C++：显式类型转换
来源：http://hz.yonumen.top/gtqcwbzfjm.html

static_cast<double>(a) / b
来源：http://hz.xziqi.cn/gtfjwdjsvh.html

[S52] C++：const 与 noexcept
来源：http://hz.9152youxi.cn/gthvuitpjz.html

int size() const noexcept { return n_; }
来源：http://hz.feifeiyinyue.top/gtznwgzccc.html

[S53] C++：移动语义
来源：http://hz.svipenyu.cn/gtqlomdriy.html

std::vector<int> w = std::move(v);
来源：http://hz.wangshuangyany.cn/gtmleifvqq.html

[S54] C++：异常处理
来源：http://hz.gaohongyu789.top/gtauwmkfqp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuanzhike.top/gtgbvzsnbz.html

[S55] C++：结构化绑定
来源：http://hz.yj202588.top/gtpebeeowg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cheryme.top/gttbkffkqg.html

[S56] C++：optional
来源：http://hz.aizwys.cn/gtqhdjqhgo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gturtpjzyb.html

[S57] C++：编译期常量
来源：http://hz.daria6918.cn/gtjpmqemhw.html

constexpr int N = 10;
来源：http://hz.yj202588.top/gtwvqfjhby.html

[S58] C++：命名空间
来源：http://hz.gogol.net.cn/gtbygobgnb.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhaomingkeji.xyz/gtshbluaqy.html

[S59] C++：静态断言
来源：http://hz.c1oappe.top/gtrismrykn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtmvruaxzn.html

[S60] C++：遍历并删除元素
来源：http://hz.ydjk.org.cn/gtcjynbpzl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.kuanghao11.cn/gthbkrkzpj.html

================================================================================
来源：http://hz.sxryk.cn/gtfrtfqunx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gogol.net.cn/gtmbbtrhky.html

================================================================================
来源：http://hz.guannengcc.top/gtedwwootn.html

[T01] Kotlin：Hello World
来源：http://hz.cashguo.top/gtggvnktzi.html

println("Hello")
来源：http://hz.haohaochexian.top/gtqpxbsold.html

[T02] Kotlin：变量
来源：http://hz.xinyue.icu/gtnmsjtwto.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sufxvd.cn/gthzabhpyv.html

[T03] Kotlin：字符串模板
来源：http://hz.havefunace.top/gtupikcgxb.html

"值: $b"
来源：http://hz.zhongyouzk.top/gtectucnzy.html

[T04] Kotlin：空安全
来源：http://hz.ydjk.org.cn/gtrmvtwrag.html

val n: String? = null;  n?.length
来源：http://hz.jlsjyb.cn/gthbyfzyat.html

[T05] Kotlin：when 表达式
来源：http://hz.shangyingyoupin.top/gtktyqxiew.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.svipenyu.cn/gttjoenwhd.html

[T06] Kotlin：集合映射
来源：http://hz.cashguo.top/gtjziodnjz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ehwqpu.com/gtbfbqkcct.html

[T07] Kotlin：集合过滤
来源：http://hz.0kj1m.cn/gtojakqydx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258888.top/gtbibidjci.html

[T08] Kotlin：数据类
来源：http://hz.snrcjt.cn/gtthzvjdwh.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtlbqcdmdo.html

[T09] Kotlin：扩展函数
来源：http://hz.hysaishi.cn/gtrhchzrra.html

fun String.exclaim() = this + "!"
来源：http://hz.zdqjudy.top/gtelllqbmb.html

[T10] Kotlin：默认参数
来源：http://hz.hnxiangtu.top/gtckijkdyn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtrkibcfjr.html

[T11] Kotlin：协程
来源：http://hz.pycfn.com/gtmkrcvawg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.vqdsnc.cn/gtqvnbzvjs.html

[T12] Kotlin：解构声明
来源：http://hz.hongshengwenyu.top/gttfzaioug.html

val (a, b) = Pair(1, 2)
来源：http://hz.feifeiyinyue.top/gtsjldcqqw.html

[T13] Kotlin：只读 Map
来源：http://hz.smart0.xyz/gtnkxmjpzd.html

val m = mapOf("a" to 1)
来源：http://hz.cucudq.cn/gtduenvtcs.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtfkturzqp.html

for (i in 1..10) println(i)
来源：http://hz.pycfn.com/gthantursc.html

[T15] Kotlin：接口
来源：http://hz.jinghuilouyu.cn/gtnvmoipia.html

interface Shape { fun area(): Double }
来源：http://hz.cucudq.cn/gtsfquqgff.html

[T16] Swift：Hello World
来源：http://hz.jiagoushi.top/gtbdivhldx.html

print("Hello")
来源：http://hz.hammf.cn/gtpymcobqm.html

[T17] Swift：变量与常量
来源：http://hz.sufxvd.cn/gtenuacjep.html

var a = 1;  let b = 2
来源：http://hz.yj202588.top/gtwriitjtv.html

[T18] Swift：字符串插值
来源：http://hz.hongshengwenyu.top/gtjceiscjw.html

"值: \(b)"
来源：http://hz.fengsongda.top/gtalpijymy.html

[T19] Swift：可选绑定
来源：http://hz.ehwqpu.com/gtcyhwtrfl.html

if let n = opt { print(n) }
来源：http://hz.xinyue.icu/gtujbefzay.html

[T20] Swift：数组操作
来源：http://hz.chenlongwang.top/gttwkjpnrz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj20258888.top/gtqzoqctzi.html

[T21] Swift：遍历
来源：http://hz.wangdashe.top/gtlhwssqzt.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtevpjbcfv.html

[T22] Swift：字典
来源：http://hz.chenjidiqi.icu/gtodyedszn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangkeji.top/gtujwjdgip.html

[T23] Swift：函数
来源：http://hz.haohaochexian.top/gtgzbrrswo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.meibo888.top/gtfpqncary.html

[T24] Swift：闭包
来源：http://hz.52xcode.cn/gtatespgrj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dashuyun.cn/gtyxqoqhey.html

[T25] Swift：结构体
来源：http://hz.kuanghao11.cn/gtgxnfjtac.html

struct P { var x: Int }
来源：http://hz.yj20258.top/gtrqrbcnnp.html

[T26] Swift：类与重写
来源：http://hz.guannengcc.top/gtphelxitz.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtlrawkzjf.html

[T27] Swift：错误处理
来源：http://hz.cucudq.cn/gtyaepkvbi.html

do { try f() } catch { print(error) }
来源：http://hz.svipenyu.cn/gtwbzvwzuk.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gtiazdtdfw.html

enum Color { case red, green }
来源：http://hz.hfpthk.cn/gtmodabevz.html

[T29] Swift：guard 提前返回
来源：http://hz.shanyushiyangkeji.top/gtotirjljr.html

guard let x = opt else { return }
来源：http://hz.zhoulong.xyz/gtqkfwiath.html

[T30] Swift：协议
来源：http://hz.jinghuilouyu.cn/gtjaimivqa.html

protocol Shape { func area() -> Double }
来源：http://hz.gzhubu.top/gttpnvgblv.html

[T31] Lua：Hello World
来源：http://hz.bjfxy.top/gtebcvkmms.html

print("Hello")
来源：http://hz.andypj.xyz/gtluhvydap.html

[T32] Lua：局部变量
来源：http://hz.yongpay.top/gtxjxwvkmv.html

local a = 1
来源：http://hz.dashuyun.cn/gtygdpomyp.html

[T33] Lua：表（数组）
来源：http://hz.redwolf501.top/gtzubqhqwn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj20258.top/gtiiiumsoj.html

[T34] Lua：遍历表
来源：http://hz.52xcode.cn/gtnieunddq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.birdmap.top/gtifhbxwng.html


<!-- 参考信息 -->