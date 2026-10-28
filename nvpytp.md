代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.yvedp.cn/gttxniovyh.html

[R32] 参数个数校验
来源：http://hz.sysykeji.top/gtthehgmbu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.quarkkingdee.top/gtxdtpttwo.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtjqssdjfp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gtowniekvy.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtmyuasrjj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxinkj.top/gtezfcgsgk.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangkeji.top/gtqezgqckq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtkugfejkp.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtnyzkygwb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhiwuduotai.top/gttvglvczt.html

[R37] 把输出赋给变量
来源：http://hz.jinqigfzy.top/gtenwftqlk.html

files=$(ls -1)
来源：http://hz.iojbl.cn/gtedetdgri.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gthnfhqrrl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sxryk.cn/gtrepjtlnq.html

[R39] 重定向标准输出与错误
来源：http://hz.0kj1m.cn/gtbkuzuzib.html

cmd > out.log 2>&1
来源：http://hz.andypj.xyz/gthsvhnusd.html

[R40] 追加写日志
来源：http://hz.sysykeji.top/gtbhjrnidt.html

echo "log" >> out.log
来源：http://hz.havefunace.top/gtoltcvnyu.html

[R41] 丢弃输出
来源：http://hz.yj20258.top/gttjlzedan.html

cmd >/dev/null 2>&1
来源：http://hz.svipenyu.cn/gtwzbwdhwi.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gtqndeblnn.html

wc -l < a.txt
来源：http://hz.yongpay.top/gttobyluck.html

[R43] 按名字查找文件
来源：http://hz.jyoumei.cn/gtamocibbb.html

find . -name "*.log" -type f
来源：http://hz.9152youxi.cn/gtdamnarkv.html

[R44] 按修改时间查找
来源：http://hz.zhongyouzk.top/gtrgpjmjbv.html

find . -mtime -7 -type f
来源：http://hz.ydjk.org.cn/gttfekazvw.html

[R45] 批量删除
来源：http://hz.yanxiufei.cn/gtqobfpurx.html

find . -name "*.tmp" -delete
来源：http://hz.fzhhl.top/gtnhtcnwiu.html

[R46] 递归替换文件内容
来源：http://hz.redwolf501.top/gtkyzujzqk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258.top/gtcoiuvryf.html

[R47] sed 单行替换
来源：http://hz.cashguo.top/gtbznhzqce.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gaohongyu789.top/gtnfwaqdya.html

[R48] awk 取指定列
来源：http://hz.jinqigufen.top/gtrtwjoskq.html

awk '{print $1, $3}' a.txt
来源：http://hz.yueranfly.top/gtoebyumid.html

[R49] awk 带条件
来源：http://hz.birdmap.top/gtrlqfjgtj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cqqwz.cn/gtstgveheu.html

[R50] awk 求和
来源：http://hz.zhaomingkeji.xyz/gtjckwmswq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtcvwhpppr.html

[R51] 排序去重取前几
来源：http://hz.chenzaomai.com/gtkibzzfwm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangtech.top/gtxghwjefl.html

[R52] 统计行数
来源：http://hz.tianlin.xyz/gttuqsybdt.html

wc -l a.txt
来源：http://hz.wangdashe.top/gtwsssqgxz.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtolrkzeyr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtajjdryvu.html

[R54] 比较两个文件
来源：http://hz.9152youxi.cn/gtyznmrehi.html

diff a.txt b.txt
来源：http://hz.tian-w.cn/gtnpyzxyox.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gttqjvyjuk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guannengcc.top/gtvxjxjtpe.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtpnxrwnkf.html

scp file user@host:/path/
来源：http://hz.andypj.xyz/gtcafpoekd.html

[R57] 远程执行命令
来源：http://hz.yvedp.cn/gtsohzmfqt.html

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtelnqloik.html

[R58] 下载文件
来源：http://hz.hongshengwenyu.top/gtgstsfapb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jiagoushi.top/gtpipngnkd.html

[R59] 发 POST JSON
来源：http://hz.shzxlz.cn/gtywnnkxcu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.mhx1999.top/gtuxrdpgxg.html

[R60] 只看 HTTP 状态码
来源：http://hz.yuxming.cn/gtiyfhbqav.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gogol.net.cn/gtkqxmfvql.html

[R61] 磁盘占用
来源：http://hz.wangdashe.top/gtlsptxhds.html

df -h;  du -sh *
来源：http://hz.wangdashe.top/gtzoaawvvx.html

[R62] 找最占空间的文件
来源：http://hz.mhx1999.top/gtgxnvucvz.html

du -ah . | sort -rh | head -10
来源：http://hz.zhongyouzk.top/gtrgaxlnbl.html

[R63] 内存与进程
来源：http://hz.yueranfly.top/gtrjrwwxek.html

free -h;  ps aux | grep nginx
来源：http://hz.kuanghao11.cn/gtjrwibpnd.html

[R64] 结束进程
来源：http://hz.bjfxy.top/gtcoawnqub.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yueranfly.top/gtdpbevcwq.html

[R65] 查看端口占用
来源：http://hz.jinqigfzy.top/gtemjfzhnd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hongshengwenyu.top/gtjjauxisk.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtxyezebxs.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtqxoblyad.html

[R67] 生成随机十六进制串
来源：http://hz.zdqjudy.top/gtupnumcfn.html

openssl rand -hex 16
来源：http://hz.svipenyu.cn/gtivjolzoy.html

[R68] 计算文件校验值
来源：http://hz.xylfe.cn/gtnwpoazed.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jyoumei.cn/gtstwaquiz.html

[R69] 生成随机密码
来源：http://hz.birdmap.top/gtchxhwist.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuetiantiany.cn/gthvvuxide.html

[R70] 时间戳与互转
来源：http://hz.bjfxy.top/gtejbalsyu.html

date +%s;  date -d @1700000000
来源：http://hz.hnqzz.top/gttlwslpmr.html

[R71] 日期格式化
来源：http://hz.sxryk.cn/gttkeyetqp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258888.top/gtrnycaace.html

[R72] 等待端口就绪
来源：http://hz.xingfuxueyuan.xyz/gtxxhjyynn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shuidangran.top/gtddfafbkl.html

[R73] 分割大日志
来源：http://hz.tanke756.top/gtndavvhha.html

split -l 1000 big.log part_
来源：http://hz.cqqwz.cn/gtmyrdkwfj.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gtmbfhfqfx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.redwolf501.top/gtpsyiqnpq.html

[R75] 导出环境变量
来源：http://hz.havefunace.top/gtyotzeryg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sysykeji.top/gtuzvhmspv.html

[R76] 使用临时文件
来源：http://hz.ehwqpu.com/gtnxbohzuc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtovagdtwf.html

[R77] 读取用户输入
来源：http://hz.jinqigfzy.top/gtopvfdbfx.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtfmqxuotw.html

[R78] 交互式菜单
来源：http://hz.sufxvd.cn/gtzcsvtoqi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cdnleiting.top/gtqxogkpcc.html

[R79] 解析命令行选项
来源：http://hz.xuanzx.com/gtwmzkzcmm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gtwrjassfp.html

[R80] 查看脚本执行耗时
来源：http://hz.aibaodan.cn/gtexvcqzak.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gtxxbjhidc.html

================================================================================
来源：http://hz.hnqzz.top/gtgimjckkm.html

S. C / C++ 专题
来源：http://hz.316326.xyz/gtdsmwmaor.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlcegmpwr.html

[S01] C：Hello World
来源：http://hz.sufxvd.cn/gthvgwtrar.html

#include <stdio.h>
来源：http://hz.wangdashe.top/gtupbsfpts.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.meibo888.top/gtqxdvshqq.html

[S02] C：变量与格式化输出
来源：http://hz.yongpay.top/gtwjljmobg.html

int a = 10; printf("%d\n", a);
来源：http://hz.gaohongyu789.top/gtxofkmhrh.html

[S03] C：读入整数
来源：http://hz.jinghuilouyu.cn/gtkgiopxkh.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gthfhukwyb.html

[S04] C：字符串复制
来源：http://hz.iojbl.cn/gtpqtzcpix.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhongyouzk.top/gtlutmbzbj.html

[S05] C：字符串长度
来源：http://hz.fengsongda.top/gtotpklply.html

strlen(s)
来源：http://hz.gogol.net.cn/gtyvtqxtoq.html

[S06] C：字符串比较
来源：http://hz.sweek.top/gtmfwsxjoh.html

strcmp(a, b) == 0
来源：http://hz.zhijiandao.cn/gthfiliywc.html

[S07] C：数组遍历求和
来源：http://hz.yangfankeji.com/gtekjtuebv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gtomoeadyt.html

[S08] C：动态内存分配与释放
来源：http://hz.shuidangran.top/gtaewjivra.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtnirxyeub.html

[S09] C：结构体定义与初始化
来源：http://hz.zhixingplan.top/gtcyhfkwhn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tanke756.top/gtnbnkxavy.html

[S10] C：指针与解引用
来源：http://hz.hongshengwenyu.top/gtuqxwhahb.html

int *p = &a;  *p = 5;
来源：http://hz.cqqwz.cn/gtnjalmirb.html

[S11] C：逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gttdnhgusf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtfaqxcgoh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangdashe.top/gtyiktmshj.html

fclose(f);
来源：http://hz.yj20258.top/gtzdowfbmc.html

[S12] C：写文件
来源：http://hz.guowangkeji.top/gtvsqxaprd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guowangkeji.top/gtwhlpaglf.html

[S13] C：宏定义
来源：http://hz.meibo888.top/gtnxumpwrl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gotoacloud.top/gtvmqtkzyj.html

[S14] C：枚举
来源：http://hz.hysaishi.cn/gtfvurchcq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zdqjudy.top/gtcsamlbzo.html

[S15] C：类型转换
来源：http://hz.gogol.net.cn/gtiazpbgnv.html

(double) a / b
来源：http://hz.cqqwz.cn/gtonihhcms.html

[S16] C：位操作置位
来源：http://hz.snrcjt.cn/gtuahryjkq.html

x |= (1 << 3);
来源：http://hz.xingfuxueyuan.xyz/gtxjuxpiou.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtuauotpvg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.0kj1m.cn/gtfstnglkg.html

[S18] C：命令行参数
来源：http://hz.gogol.net.cn/gtebkodzij.html

int main(int argc, char **argv)
来源：http://hz.birdmap.top/gtlgjzrkyr.html

[S19] C：快速排序
来源：http://hz.ivvv.top/gtvwwvykyz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtlpyzmczh.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtvtkkivue.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtkhrsobws.html

[S21] C：字符类别判断
来源：http://hz.jlsjyb.cn/gtrkicsjcj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hammf.cn/gtkqrvaxqs.html

[S22] C：字符串转数字
来源：http://hz.zhiwuduotai.top/gtbuuzxlym.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgfzy.top/gtfthyqmpk.html

[S23] C：随机数
来源：http://hz.hywenlv.cn/gtsuxduaqo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.svipenyu.cn/gtwykcvbce.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangtech.top/gtovchsbrp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jiagoushi.top/gtrlcgpnva.html

[S25] C：内存拷贝
来源：http://hz.jyoumei.cn/gthmgdhdbg.html

memcpy(dst, src, n);
来源：http://hz.kuanghao11.cn/gtnmlhfcxc.html

[S26] C：内存清零
来源：http://hz.kuanghao11.cn/gtdwrcffsh.html

memset(a, 0, sizeof a);
来源：http://hz.daxiang520.top/gtavdlazum.html

[S27] C：定义常量
来源：http://hz.yvedp.cn/gtxufzuapv.html

const double PI = 3.14159;
来源：http://hz.birdmap.top/gtlbosxosk.html

[S28] C：静态变量
来源：http://hz.yongpay.top/gtequsrcln.html

static int counter = 0;
来源：http://hz.zycfv.cn/gtdbwwceml.html

[S29] C：变参函数
来源：http://hz.tianlin.xyz/gtjbktygep.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhijiandao.cn/gtyfrvnoda.html

[S30] C：头文件保护
来源：http://hz.hnxiangtu.top/gtbkuutxae.html

#ifndef X_H
来源：http://hz.9152youxi.cn/gtrxqzowno.html

#define X_H
来源：http://hz.hammf.cn/gtcdfuwuqq.html

#endif
来源：http://hz.zdqjudy.top/gtgipswnpx.html

[S31] C++：Hello World
来源：http://hz.quarkkingdee.top/gtfinhgohc.html

#include <iostream>
来源：http://hz.meibo888.top/gtbyluztqm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigufen.top/gtsrmyyncc.html

[S32] C++：字符串
来源：http://hz.nwbrower.top/gtyjoqfrzf.html

std::string s = "hi";  s += "!";
来源：http://hz.hammf.cn/gtmugcywpd.html

[S33] C++：vector 增删
来源：http://hz.ydzc1.top/gtjexxpfwq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hfpthk.cn/gtjlfloxfj.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtzorrgrlt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gtpyjjyzyg.html

[S35] C++：map
来源：http://hz.shzxlz.cn/gtkjvilxxb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtyrwgdjqi.html

[S36] C++：unordered_map
来源：http://hz.shangyingyoupin.top/gtoaldyvjg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtaugzbwlm.html

[S37] C++：set
来源：http://hz.52xcode.cn/gteaipvhjh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gzhubu.top/gtxpjbgukl.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtqazwkpdn.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtguuigzyi.html

[S39] C++：自定义比较器排序
来源：http://hz.guannengcc.top/gtxftompgl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.meibo888.top/gtwdqsnjoz.html

[S40] C++：查找元素
来源：http://hz.chenlongwang.top/gtybxqpkac.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sufxvd.cn/gterspsxcv.html

[S41] C++：类与构造函数
来源：http://hz.iojbl.cn/gtzlevjwvn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtjlbjdrcy.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gttieibumi.html

class B : public Base { public: void f() override {} };
来源：http://hz.hfpthk.cn/gtxezvmryn.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gtxiwqmytk.html

auto p = std::make_unique<int>(5);
来源：http://hz.quarkkingdee.top/gtdobcmcwd.html

[S44] C++：引用传参
来源：http://hz.xuetiantiany.cn/gtmyqeckyn.html

void inc(int &x) { ++x; }
来源：http://hz.jyoumei.cn/gtnmztbxam.html

[S45] C++：lambda
来源：http://hz.ydjk.org.cn/gtzjwffmet.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gthdswsekk.html

[S46] C++：函数模板
来源：http://hz.hongshengwenyu.top/gtechqqfze.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtpjuhmhkh.html

[S47] C++：结构化绑定遍历
来源：http://hz.meibo888.top/gtisoaunik.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.bjfxy.top/gtntubwnja.html

[S48] C++：逐行读文件
来源：http://hz.chenzaomai.com/gtzsoevkst.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gtwwlczico.html

while (std::getline(in, line)) { }
来源：http://hz.wangdashe.top/gtkvrormts.html

[S49] C++：写文件
来源：http://hz.xuetiantiany.cn/gtiveylyfh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sxryk.cn/gtvllndrzx.html

[S50] C++：格式化数字
来源：http://hz.shangyingyoupin.top/gtxznofzil.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jlsjyb.cn/gtwpghrmox.html

[S51] C++：显式类型转换
来源：http://hz.chenjidiqi.icu/gtmkpyssta.html

static_cast<double>(a) / b
来源：http://hz.yvedp.cn/gttgtwdkpa.html

[S52] C++：const 与 noexcept
来源：http://hz.tanke756.top/gtzxamplhs.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gthxenqfix.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gthbxmegey.html

std::vector<int> w = std::move(v);
来源：http://hz.haohaochexian.top/gtrhdhxugs.html

[S54] C++：异常处理
来源：http://hz.wangshuangyany.cn/gtahpbseld.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.meibo888.top/gtruomaztc.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gttnabbjlh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xylfe.cn/gthymzyzst.html

[S56] C++：optional
来源：http://hz.316326.xyz/gtgeeiubpj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangtech.top/gtlielfjdw.html

[S57] C++：编译期常量
来源：http://hz.shuidangran.top/gtrsnsbzph.html

constexpr int N = 10;
来源：http://hz.jqgfzy.top/gtrdemuoac.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gthjopeuyc.html

namespace ns { int f() { return 1; } }
来源：http://hz.iojbl.cn/gtnkvscsjo.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtozlbnktp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenjidiqi.icu/gtejysnmbx.html

[S60] C++：遍历并删除元素
来源：http://hz.bjfxy.top/gtnwohnspm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ppjwa.cn/gtkystqgtu.html

================================================================================
来源：http://hz.jinqigufen.top/gtnhsxeszh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigufen.top/gtugjdvtcf.html

================================================================================
来源：http://hz.yj20258.top/gtoqanmvlt.html

[T01] Kotlin：Hello World
来源：http://hz.shzxlz.cn/gtfhjlgkog.html

println("Hello")
来源：http://hz.fengsongda.top/gttcyezxkb.html

[T02] Kotlin：变量
来源：http://hz.zycfv.cn/gthsctaewr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hysaishi.cn/gtjsnuvbht.html

[T03] Kotlin：字符串模板
来源：http://hz.pengpengdd.cyou/gtcatxtbfk.html

"值: $b"
来源：http://hz.snrcjt.cn/gtboxhlpzw.html

[T04] Kotlin：空安全
来源：http://hz.zhixingplan.top/gtratwisur.html

val n: String? = null;  n?.length
来源：http://hz.jinqigfzy.top/gtjlnkiqdi.html

[T05] Kotlin：when 表达式
来源：http://hz.cucudq.cn/gtanlcaubm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigufen.top/gtfvasukbr.html

[T06] Kotlin：集合映射
来源：http://hz.ppjwa.cn/gthjiqoyrn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sweek.top/gtydzqjsen.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258.top/gtyeskqbnr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xziqi.cn/gtzorcfsgi.html

[T08] Kotlin：数据类
来源：http://hz.sweek.top/gtlozcnarj.html

data class User(val name: String, val age: Int)
来源：http://hz.gzhubu.top/gtllptyedy.html

[T09] Kotlin：扩展函数
来源：http://hz.gzhubu.top/gtewcydxbh.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtewtvhbin.html

[T10] Kotlin：默认参数
来源：http://hz.fzhhl.top/gtfkrcslcq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gtdlmtqemw.html

[T11] Kotlin：协程
来源：http://hz.xuetiantiany.cn/gtkkqkxjvt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tian-w.cn/gtkyulzyfs.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtozroemaz.html

val (a, b) = Pair(1, 2)
来源：http://hz.iojbl.cn/gtokgyahhc.html

[T13] Kotlin：只读 Map
来源：http://hz.ivvv.top/gticanomcy.html

val m = mapOf("a" to 1)
来源：http://hz.gaohongyu789.top/gtkawpevbs.html

[T14] Kotlin：循环
来源：http://hz.wangdashe.top/gtkxkzcjxx.html

for (i in 1..10) println(i)
来源：http://hz.yueranfly.top/gtwerpsvri.html

[T15] Kotlin：接口
来源：http://hz.redwolf501.top/gtzdlpoynm.html

interface Shape { fun area(): Double }
来源：http://hz.yonumen.top/gtcnikweef.html

[T16] Swift：Hello World
来源：http://hz.ywan-chungtsiang.top/gtzcrjrnay.html

print("Hello")
来源：http://hz.daxiang520.top/gtdlojsvwk.html

[T17] Swift：变量与常量
来源：http://hz.guowangkeji.top/gtutbxuxib.html

var a = 1;  let b = 2
来源：http://hz.xingfuxueyuan.xyz/gtkwlfrpbu.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtjkfuzjcb.html

"值: \(b)"
来源：http://hz.zdqjudy.top/gtsxqccoxd.html

[T19] Swift：可选绑定
来源：http://hz.yuxming.cn/gteejgkxzv.html

if let n = opt { print(n) }
来源：http://hz.feifeiyinyue.top/gtpdgnpjoo.html

[T20] Swift：数组操作
来源：http://hz.smart0.xyz/gtuazuxonw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aibaodan.cn/gtzkgntmwi.html

[T21] Swift：遍历
来源：http://hz.sxryk.cn/gtqqzbyfem.html

for x in a { print(x) }
来源：http://hz.jinghuilouyu.cn/gtlpcucujy.html

[T22] Swift：字典
来源：http://hz.hywenlv.cn/gtlgxvrgot.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tanke756.top/gtpsdrotqn.html

[T23] Swift：函数
来源：http://hz.ydjk.org.cn/gtxbgwiffi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ehwqpu.com/gtmgsmllpg.html

[T24] Swift：闭包
来源：http://hz.xziqi.cn/gtnaohpcnn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtysizwjli.html

[T25] Swift：结构体
来源：http://hz.xingfuxueyuan.xyz/gtgwhjztgd.html

struct P { var x: Int }
来源：http://hz.haohaochexian.top/gthwlznipb.html

[T26] Swift：类与重写
来源：http://hz.haohaochexian.top/gtlzftdrxs.html

class A: Base { override func f() {} }
来源：http://hz.kuanghao11.cn/gtvqjhznac.html

[T27] Swift：错误处理
来源：http://hz.tian-w.cn/gtqllbkmiz.html

do { try f() } catch { print(error) }
来源：http://hz.dashuyun.cn/gtlprjifoq.html

[T28] Swift：枚举
来源：http://hz.zhiwuduotai.top/gtbutliohv.html

enum Color { case red, green }
来源：http://hz.iojbl.cn/gtzhislful.html

[T29] Swift：guard 提前返回
来源：http://hz.hnxiangtu.top/gtgxnsiqaa.html

guard let x = opt else { return }
来源：http://hz.cheryme.top/gtgqpobigd.html

[T30] Swift：协议
来源：http://hz.jinqigfzy.top/gttpxqsehr.html

protocol Shape { func area() -> Double }
来源：http://hz.shuidangran.top/gtclzuzqss.html

[T31] Lua：Hello World
来源：http://hz.9152youxi.cn/gtzadmxirk.html

print("Hello")
来源：http://hz.cqqwz.cn/gtqbxqlgoh.html

[T32] Lua：局部变量
来源：http://hz.ybcxt.top/gtyqpuffni.html

local a = 1
来源：http://hz.shuidangran.top/gtsmhqxrhh.html

[T33] Lua：表（数组）
来源：http://hz.yj20258.top/gtmfhnduss.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.kuanghao11.cn/gtiiyayxcb.html

[T34] Lua：遍历表
来源：http://hz.daria6918.cn/gtpactzkyg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtuuognorf.html


<!-- 参考信息 -->