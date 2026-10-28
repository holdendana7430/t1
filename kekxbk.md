代发 wailian999

echo $((1 + 2 * 3))
来源：http://hz.ivvv.top/gtvyupdcgk.html

[R28] 浮点运算
来源：http://hz.xinyue.icu/gttcwqzufp.html

echo "scale=2; 10/3" | bc
来源：http://hz.ybcxt.top/gthrfiegqx.html

[R29] 定义函数
来源：http://hz.c1oappe.top/gtzfwilnus.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cqqwz.cn/gtntixcejx.html

[R30] 函数返回状态码
来源：http://hz.xinyue.icu/gtggldtgef.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gzhubu.top/gtkufwzigc.html

[R31] 局部变量
来源：http://hz.jqgufenzy.top/gtzwazzdru.html

f() { local x=1; echo "$x"; }
来源：http://hz.aizwys.cn/gtscynvkgd.html

[R32] 参数个数校验
来源：http://hz.zhijiandao.cn/gtnolhzzyc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgfzy.top/gtmanvafuo.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258888.top/gttevylqka.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.9152youxi.cn/gtnoovfyec.html

[R34] 退出时清理
来源：http://hz.ywan-chungtsiang.top/gtdwbjltob.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtnkcnjpmj.html

[R35] 后台执行并等待
来源：http://hz.cashguo.top/gtbpcfmagj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sufxvd.cn/gtmswklgmp.html

[R36] 并发执行多个任务
来源：http://hz.mhx1999.top/gtwjixoypo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gtliruozrp.html

[R37] 把输出赋给变量
来源：http://hz.jiagoushi.top/gtpgdfgkpf.html

files=$(ls -1)
来源：http://hz.cheryme.top/gtgsctiavo.html

[R38] 管道串联
来源：http://hz.yj20258888.top/gtxggxkzjl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinqigfzy.top/gtdnrmfjlc.html

[R39] 重定向标准输出与错误
来源：http://hz.hammf.cn/gtzlxjcwqf.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gtjftoizfr.html

[R40] 追加写日志
来源：http://hz.sxryk.cn/gtswiezrhr.html

echo "log" >> out.log
来源：http://hz.gogol.net.cn/gtvehndzry.html

[R41] 丢弃输出
来源：http://hz.tianlin.xyz/gtkfqwrcoq.html

cmd >/dev/null 2>&1
来源：http://hz.tanke756.top/gteeuptkyq.html

[R42] 输入重定向
来源：http://hz.redwolf501.top/gtxogvyzna.html

wc -l < a.txt
来源：http://hz.jianghu66.top/gttkygmfmg.html

[R43] 按名字查找文件
来源：http://hz.ydzc1.top/gtqmnfuwdr.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtwhxhdnsl.html

[R44] 按修改时间查找
来源：http://hz.snrcjt.cn/gttjiprpzo.html

find . -mtime -7 -type f
来源：http://hz.pengpengdd.cyou/gtvcikyyqe.html

[R45] 批量删除
来源：http://hz.jinqigfzy.top/gtnrdcpdgu.html

find . -name "*.tmp" -delete
来源：http://hz.yanxiufei.cn/gtezadxwyv.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gtciovauwm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtgcfcmibq.html

[R47] sed 单行替换
来源：http://hz.wangdashe.top/gtikesdvye.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yueranfly.top/gtvkomafbd.html

[R48] awk 取指定列
来源：http://hz.chenzaomai.com/gtfkwprlbk.html

awk '{print $1, $3}' a.txt
来源：http://hz.iojbl.cn/gthuowczyf.html

[R49] awk 带条件
来源：http://hz.yangfankeji.com/gtadeefdfh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cucudq.cn/gtiwzphfrk.html

[R50] awk 求和
来源：http://hz.ybcxt.top/gtrtpyyxda.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtrqzyrdws.html

[R51] 排序去重取前几
来源：http://hz.tian-w.cn/gtfiutbzoq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhongyouzk.top/gtgpvyazlk.html

[R52] 统计行数
来源：http://hz.aibaodan.cn/gtmvazqaab.html

wc -l a.txt
来源：http://hz.redwolf501.top/gtwxhbmxhh.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtdktbegdo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gzhubu.top/gtevjurgtf.html

[R54] 比较两个文件
来源：http://hz.ydjk.org.cn/gtisknhwpt.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtjeggowaq.html

[R55] 压缩与解压
来源：http://hz.zhaomingkeji.xyz/gtnhxndoge.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dianchejie.cn/gtodbqkrco.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gtgpiygvvv.html

scp file user@host:/path/
来源：http://hz.guowangkeji.top/gtcrrghbaw.html

[R57] 远程执行命令
来源：http://hz.ehwqpu.com/gtiewmcddl.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtyuwfzvns.html

[R58] 下载文件
来源：http://hz.gotoacloud.top/gtquzdzomp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gotoacloud.top/gttmktmeps.html

[R59] 发 POST JSON
来源：http://hz.xuetiantiany.cn/gtnocpahmz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.snrcjt.cn/gtzvztiwpn.html

[R60] 只看 HTTP 状态码
来源：http://hz.xylfe.cn/gtgfbgemko.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xingfuxueyuan.xyz/gtmuflodco.html

[R61] 磁盘占用
来源：http://hz.gzhubu.top/gtjuqyyagk.html

df -h;  du -sh *
来源：http://hz.xziqi.cn/gtgfnodlkz.html

[R62] 找最占空间的文件
来源：http://hz.ybcxt.top/gtzvwbewcr.html

du -ah . | sort -rh | head -10
来源：http://hz.cqqwz.cn/gtmhthvtww.html

[R63] 内存与进程
来源：http://hz.dashuyun.cn/gtniepuxyf.html

free -h;  ps aux | grep nginx
来源：http://hz.cqqwz.cn/gtjdfmollh.html

[R64] 结束进程
来源：http://hz.tianlin.xyz/gtjkssxfkb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hfpthk.cn/gtmqwzheqb.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangkeji.top/gthrhwszqm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigfzy.top/gtyrvjofam.html

[R66] 定时任务
来源：http://hz.hywenlv.cn/gttyxgsesp.html

crontab -e;  crontab -l
来源：http://hz.jiagoushi.top/gttfsjypgm.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtlezgsyuy.html

openssl rand -hex 16
来源：http://hz.shangyingyoupin.top/gtxytwwsou.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtocsfbkyo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.iojbl.cn/gtqfkbougf.html

[R69] 生成随机密码
来源：http://hz.wangdashe.top/gtwiekojls.html

head -c 16 /dev/urandom | base64
来源：http://hz.9152youxi.cn/gtkipikcek.html

[R70] 时间戳与互转
来源：http://hz.kuanghao11.cn/gtduynryud.html

date +%s;  date -d @1700000000
来源：http://hz.yongpay.top/gtvadvbuhn.html

[R71] 日期格式化
来源：http://hz.xuanzx.com/gtjyxytmtf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtjpfrwcpt.html

[R72] 等待端口就绪
来源：http://hz.ppjwa.cn/gtxoihyxga.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gtnrnokako.html

[R73] 分割大日志
来源：http://hz.gzhubu.top/gtonkcmmgs.html

split -l 1000 big.log part_
来源：http://hz.jinqigfzy.top/gtgmxdljyy.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gtclzasuov.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.wangdashe.top/gtkfrnigrb.html

[R75] 导出环境变量
来源：http://hz.zhijiandao.cn/gtjwnrgonr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtgovvudrt.html

[R76] 使用临时文件
来源：http://hz.gogol.net.cn/gtoipgdown.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gthwdwxxyv.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtzubijhsg.html

read -rp "请输入: " ans
来源：http://hz.zhongyouzk.top/gtjuufenyt.html

[R78] 交互式菜单
来源：http://hz.zhongyouzk.top/gtuwpzmtte.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hywenlv.cn/gtpvqxkldl.html

[R79] 解析命令行选项
来源：http://hz.hfpthk.cn/gtyszbvuos.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.316326.xyz/gtupqknvkt.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtdbtqbvby.html

time ./run.sh
来源：http://hz.ivvv.top/gtqrscbfvx.html

================================================================================
来源：http://hz.tanke756.top/gtsxcuupfv.html

S. C / C++ 专题
来源：http://hz.yongpay.top/gtzajslynb.html

================================================================================
来源：http://hz.cheryme.top/gtdbgurfdj.html

[S01] C：Hello World
来源：http://hz.sysykeji.top/gthzywntld.html

#include <stdio.h>
来源：http://hz.shzxlz.cn/gtonhyvdae.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jianghu66.top/gtsixbbikt.html

[S02] C：变量与格式化输出
来源：http://hz.chenzaomai.com/gthpavqlhg.html

int a = 10; printf("%d\n", a);
来源：http://hz.xingfuxueyuan.xyz/gtfyoxteyf.html

[S03] C：读入整数
来源：http://hz.tianlin.xyz/gtlwqipzcf.html

int x; scanf("%d", &x);
来源：http://hz.sweek.top/gtzitogjfg.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtdqldniix.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xinyue.icu/gtyeguxmge.html

[S05] C：字符串长度
来源：http://hz.ivvv.top/gtjtnfxcrr.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gtxjokfcfm.html

[S06] C：字符串比较
来源：http://hz.yuanzhike.top/gtcytqjcqp.html

strcmp(a, b) == 0
来源：http://hz.pengpengdd.cyou/gtarcqwtws.html

[S07] C：数组遍历求和
来源：http://hz.chenjidiqi.icu/gteymlfctf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhongyouzk.top/gtxsixubkv.html

[S08] C：动态内存分配与释放
来源：http://hz.mhx1999.top/gthtwaexup.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenzaomai.com/gtyrlxbcxd.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258.top/gtzozvbzbn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.kuanghao11.cn/gtditatvov.html

[S10] C：指针与解引用
来源：http://hz.yuanzhike.top/gtyxokzzyv.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtisbhhlcl.html

[S11] C：逐行读文件
来源：http://hz.iojbl.cn/gthpoheyui.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.mhx1999.top/gtbnvqxdqj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gtwikexxcv.html

fclose(f);
来源：http://hz.xuanzx.com/gthktunoxb.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtawthqcjj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenzaomai.com/gttmpjbhoy.html

[S13] C：宏定义
来源：http://hz.yuanzhike.top/gtigllnvwp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtppmolgta.html

[S14] C：枚举
来源：http://hz.gzhubu.top/gtlhxdkfvm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.redwolf501.top/gtihrlqnkl.html

[S15] C：类型转换
来源：http://hz.shanyushiyangtech.top/gtddfmvwkp.html

(double) a / b
来源：http://hz.chenzaomai.com/gtwazdpreg.html

[S16] C：位操作置位
来源：http://hz.xuanzx.com/gtpyyiznpt.html

x |= (1 << 3);
来源：http://hz.chenlongwang.top/gtqlsuvlzq.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtfzbhlajs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhoulong.xyz/gtepmlqwig.html

[S18] C：命令行参数
来源：http://hz.kuanghao11.cn/gtbriuvhci.html

int main(int argc, char **argv)
来源：http://hz.zhixingplan.top/gtpaehwmmh.html

[S19] C：快速排序
来源：http://hz.guannengcc.top/gtiroynnuj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtpwzpzsli.html

[S20] C：二分查找
来源：http://hz.52xcode.cn/gtooaufpzh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtfgknslko.html

[S21] C：字符类别判断
来源：http://hz.gaohongyu789.top/gtltquzdqg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hywenlv.cn/gttlgonwke.html

[S22] C：字符串转数字
来源：http://hz.ywan-chungtsiang.top/gtindezvvk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.iojbl.cn/gtehbqubns.html

[S23] C：随机数
来源：http://hz.jiagoushi.top/gtodtbhihb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cdnleiting.top/gtsdwlital.html

[S24] C：获取本地时间
来源：http://hz.9152youxi.cn/gtwbciasgs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.mhx1999.top/gtyulxhbtw.html

[S25] C：内存拷贝
来源：http://hz.ywan-chungtsiang.top/gtszcgtndw.html

memcpy(dst, src, n);
来源：http://hz.jinqigufen.top/gtjenrymga.html

[S26] C：内存清零
来源：http://hz.pengpengdd.cyou/gtyplmmwxg.html

memset(a, 0, sizeof a);
来源：http://hz.xylfe.cn/gthvtlbrxv.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtixoetrhe.html

const double PI = 3.14159;
来源：http://hz.jianghu66.top/gtbwwnvruv.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gthbagbxfh.html

static int counter = 0;
来源：http://hz.316326.xyz/gtxihhvbfs.html

[S29] C：变参函数
来源：http://hz.hysaishi.cn/gtmxhnwvfo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhiwuduotai.top/gtdhywbmct.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtszlkyzev.html

#ifndef X_H
来源：http://hz.yongpay.top/gthnywjduy.html

#define X_H
来源：http://hz.kuanghao11.cn/gtnapdhirb.html

#endif
来源：http://hz.svipenyu.cn/gtsqzqnwkz.html

[S31] C++：Hello World
来源：http://hz.yonumen.top/gtwgaczlkx.html

#include <iostream>
来源：http://hz.zhoulong.xyz/gtqblkcues.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ybcxt.top/gtjjkumedg.html

[S32] C++：字符串
来源：http://hz.zhaomingkeji.xyz/gtypsipbrm.html

std::string s = "hi";  s += "!";
来源：http://hz.fzhhl.top/gtjmsadhef.html

[S33] C++：vector 增删
来源：http://hz.yj20258.top/gtmrfsfmlg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sysykeji.top/gtedwvrorn.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtozybtliz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daria6918.cn/gtftwjipdq.html

[S35] C++：map
来源：http://hz.zhixingplan.top/gtoewcdyyc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtimxzjrgc.html

[S36] C++：unordered_map
来源：http://hz.sweek.top/gtwkxjnmfw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtwnbdmcbq.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtqfusnfsl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnxiangtu.top/gtjzfvqtqy.html

[S38] C++：排序
来源：http://hz.quarkkingdee.top/gtnvcupxgg.html

std::sort(v.begin(), v.end());
来源：http://hz.hywenlv.cn/gtedigkmrt.html

[S39] C++：自定义比较器排序
来源：http://hz.wangdashe.top/gtriwnhbul.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ywan-chungtsiang.top/gtegsmmjac.html

[S40] C++：查找元素
来源：http://hz.gogol.net.cn/gtmtvvjofi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fengsongda.top/gtyeewwwtq.html

[S41] C++：类与构造函数
来源：http://hz.nanxinkj.top/gtleuxkmkm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.snrcjt.cn/gtnfouuerr.html

[S42] C++：继承与虚函数
来源：http://hz.yangfankeji.com/gtnpspllws.html

class B : public Base { public: void f() override {} };
来源：http://hz.c1oappe.top/gtuarvrjtz.html

[S43] C++：智能指针
来源：http://hz.nwbrower.top/gtnteqheiq.html

auto p = std::make_unique<int>(5);
来源：http://hz.guannengcc.top/gtckitbyrh.html

[S44] C++：引用传参
来源：http://hz.yuxming.cn/gtucrdyilk.html

void inc(int &x) { ++x; }
来源：http://hz.ydzc1.top/gtuybggwni.html

[S45] C++：lambda
来源：http://hz.cashguo.top/gtwcgzowch.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gtvqarhmov.html

[S46] C++：函数模板
来源：http://hz.aibaodan.cn/gtwsnimlik.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258888.top/gtqnplfcsx.html

[S47] C++：结构化绑定遍历
来源：http://hz.shuidangran.top/gtkwcrdxtc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenjidiqi.icu/gtbnqzlvmb.html

[S48] C++：逐行读文件
来源：http://hz.iojbl.cn/gtpgwurugo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xylfe.cn/gtqpxsoecl.html

while (std::getline(in, line)) { }
来源：http://hz.yueranfly.top/gtdgvivmcz.html

[S49] C++：写文件
来源：http://hz.c1oappe.top/gtkfotirem.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yangfankeji.com/gtenxronxu.html

[S50] C++：格式化数字
来源：http://hz.zhijiandao.cn/gtvowwkqxs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zdqjudy.top/gtqprfsmuc.html

[S51] C++：显式类型转换
来源：http://hz.yj20258888.top/gttspneknn.html

static_cast<double>(a) / b
来源：http://hz.hnqzz.top/gtoivuerwx.html

[S52] C++：const 与 noexcept
来源：http://hz.gotoacloud.top/gtvfakhjps.html

int size() const noexcept { return n_; }
来源：http://hz.zhixingplan.top/gtgnexxvdi.html

[S53] C++：移动语义
来源：http://hz.ywan-chungtsiang.top/gtpfbajfqz.html

std::vector<int> w = std::move(v);
来源：http://hz.zhongyouzk.top/gtubtckdvy.html

[S54] C++：异常处理
来源：http://hz.pengpengdd.cyou/gtzyywgljz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jyoumei.cn/gtcfwadqwd.html

[S55] C++：结构化绑定
来源：http://hz.hnxiangtu.top/gtyvjikfpb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zycfv.cn/gtkkfoxuwo.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gtaxktfrfm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cashguo.top/gtduobjllm.html

[S57] C++：编译期常量
来源：http://hz.dashuyun.cn/gtfsetfhbk.html

constexpr int N = 10;
来源：http://hz.shanyushiyangkeji.top/gtwsphsreq.html

[S58] C++：命名空间
来源：http://hz.chenzaomai.com/gtjkjhmqzz.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxinkj.top/gttjuipzeg.html

[S59] C++：静态断言
来源：http://hz.haohaochexian.top/gttxroslcb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.dianchejie.cn/gtlsnfijyg.html

[S60] C++：遍历并删除元素
来源：http://hz.hammf.cn/gtvibdxmuk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sysykeji.top/gthlwasckq.html

================================================================================
来源：http://hz.pycfn.com/gtkkqgadkn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigfzy.top/gtgpodfryu.html

================================================================================
来源：http://hz.zhengqikj.top/gttkzuxpqt.html

[T01] Kotlin：Hello World
来源：http://hz.shzxlz.cn/gtifmvuhql.html

println("Hello")
来源：http://hz.redwolf501.top/gtthpgfsuo.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gttgijzxxb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aizwys.cn/gteevwhgdw.html

[T03] Kotlin：字符串模板
来源：http://hz.52xcode.cn/gtfugkcklz.html

"值: $b"
来源：http://hz.yj202588.top/gtxmjsicqp.html

[T04] Kotlin：空安全
来源：http://hz.haohaochexian.top/gtlajrwxpj.html

val n: String? = null;  n?.length
来源：http://hz.yongpay.top/gtlaqwxmjf.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gtgdfimzze.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yueranfly.top/gtesufmyyx.html

[T06] Kotlin：集合映射
来源：http://hz.andypj.xyz/gtzevacrbs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj20258888.top/gteilzpbug.html

[T07] Kotlin：集合过滤
来源：http://hz.0kj1m.cn/gtgendxden.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.snrcjt.cn/gtuofkkdzb.html

[T08] Kotlin：数据类
来源：http://hz.cheryme.top/gtyenejjtv.html

data class User(val name: String, val age: Int)
来源：http://hz.xuetiantiany.cn/gthzancouq.html

[T09] Kotlin：扩展函数
来源：http://hz.52xcode.cn/gtqtvnlvxh.html

fun String.exclaim() = this + "!"
来源：http://hz.hnxiangtu.top/gtobgmrrfw.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gttaizzyzy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xziqi.cn/gtphpjvdhb.html

[T11] Kotlin：协程
来源：http://hz.ppjwa.cn/gtvlnqdqpr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinghuilouyu.cn/gtyshjxrco.html

[T12] Kotlin：解构声明
来源：http://hz.pycfn.com/gtqxfhcdpx.html

val (a, b) = Pair(1, 2)
来源：http://hz.meibo888.top/gtpqlmitby.html

[T13] Kotlin：只读 Map
来源：http://hz.0kj1m.cn/gtyizsuloh.html

val m = mapOf("a" to 1)
来源：http://hz.hnxiangtu.top/gtkpyvgqje.html

[T14] Kotlin：循环
来源：http://hz.jlsjyb.cn/gtxpgmxxsy.html

for (i in 1..10) println(i)
来源：http://hz.ppjwa.cn/gtpqamtpvb.html

[T15] Kotlin：接口
来源：http://hz.daria6918.cn/gtbjdartfc.html

interface Shape { fun area(): Double }
来源：http://hz.quarkkingdee.top/gtgmjaszxz.html

[T16] Swift：Hello World
来源：http://hz.c1oappe.top/gtmmvuwrdd.html

print("Hello")
来源：http://hz.guowangkeji.top/gtdjkxbvin.html

[T17] Swift：变量与常量
来源：http://hz.aizwys.cn/gtltrevaie.html

var a = 1;  let b = 2
来源：http://hz.52xcode.cn/gtbnrkbrnf.html

[T18] Swift：字符串插值
来源：http://hz.smart0.xyz/gtsiffbpnn.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtyvgnfebp.html

[T19] Swift：可选绑定
来源：http://hz.shangyingyoupin.top/gtxebcjzct.html

if let n = opt { print(n) }
来源：http://hz.meibo888.top/gtyqhocbrh.html

[T20] Swift：数组操作
来源：http://hz.hywenlv.cn/gtmsqycsds.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ybcxt.top/gtogksefdk.html

[T21] Swift：遍历
来源：http://hz.ehwqpu.com/gtucjomofj.html

for x in a { print(x) }
来源：http://hz.zhoulong.xyz/gtvkyvsyhr.html

[T22] Swift：字典
来源：http://hz.zhixingplan.top/gtjkjrgotf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhiwuduotai.top/gtrmrlhckc.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtmrdisqvj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tianlin.xyz/gtjyxyxcej.html

[T24] Swift：闭包
来源：http://hz.zhoulong.xyz/gtijaekbqg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yanxiufei.cn/gtcylqitpc.html

[T25] Swift：结构体
来源：http://hz.ehwqpu.com/gtyayzoxqk.html

struct P { var x: Int }
来源：http://hz.shanyushiyangtech.top/gtdsnosdvm.html

[T26] Swift：类与重写
来源：http://hz.wangshuangyany.cn/gtnkpmowfd.html

class A: Base { override func f() {} }
来源：http://hz.pengpengdd.cyou/gtmfbpjdka.html

[T27] Swift：错误处理
来源：http://hz.wangshuangyany.cn/gtzvjcqwmt.html

do { try f() } catch { print(error) }
来源：http://hz.nwbrower.top/gtuujviuzk.html

[T28] Swift：枚举
来源：http://hz.chenzaomai.com/gtgaodlxep.html

enum Color { case red, green }
来源：http://hz.hysaishi.cn/gtybsljeel.html

[T29] Swift：guard 提前返回
来源：http://hz.sufxvd.cn/gtmzhaqpxk.html

guard let x = opt else { return }
来源：http://hz.yj20258888.top/gtvbvbotpa.html

[T30] Swift：协议
来源：http://hz.gotoacloud.top/gtjpqwwtgw.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gtpztuovdm.html


<!-- 参考信息 -->