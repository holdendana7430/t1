代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gtpvarytvg.html

[R30] 函数返回状态码
来源：http://hz.zhijiandao.cn/gtpgafpshl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtdycfhqjv.html

[R31] 局部变量
来源：http://hz.tianlin.xyz/gtpzjixfdb.html

f() { local x=1; echo "$x"; }
来源：http://hz.52xcode.cn/gtzylosnff.html

[R32] 参数个数校验
来源：http://hz.tianlin.xyz/gtgesimuwp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xylfe.cn/gtprexzaem.html

[R33] 捕获错误并提示行号
来源：http://hz.zhixingplan.top/gtjmrbhuyn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxuanxn.top/gtbxksorpx.html

[R34] 退出时清理
来源：http://hz.jinqigufen.top/gtqcpaxxfg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtdexqscnv.html

[R35] 后台执行并等待
来源：http://hz.c1oappe.top/gtjbyrkjpc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fengsongda.top/gtfnpvbjth.html

[R36] 并发执行多个任务
来源：http://hz.sweek.top/gtewtyaups.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.svipenyu.cn/gtmmsucgpk.html

[R37] 把输出赋给变量
来源：http://hz.redwolf501.top/gtfhqvpgoi.html

files=$(ls -1)
来源：http://hz.chenzaomai.com/gtomfvucdx.html

[R38] 管道串联
来源：http://hz.chenjidiqi.icu/gtfgbygqwf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.smart0.xyz/gtjakkqjvn.html

[R39] 重定向标准输出与错误
来源：http://hz.redwolf501.top/gtuscyufuy.html

cmd > out.log 2>&1
来源：http://hz.shuidangran.top/gtmovjncit.html

[R40] 追加写日志
来源：http://hz.hnxiangtu.top/gtuxunbuwh.html

echo "log" >> out.log
来源：http://hz.xuanzx.com/gtbguvbzxm.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gthqqlgnvw.html

cmd >/dev/null 2>&1
来源：http://hz.shuidangran.top/gtmcuydnxn.html

[R42] 输入重定向
来源：http://hz.nanxuanxn.top/gthkpliqai.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtrlqzvdnf.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtbolnamgi.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtnasupjdi.html

[R44] 按修改时间查找
来源：http://hz.ydzc1.top/gtsdhcgilj.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtmkpbgixj.html

[R45] 批量删除
来源：http://hz.wangshuangyany.cn/gtkqanoanf.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtvbqylpvo.html

[R46] 递归替换文件内容
来源：http://hz.sysykeji.top/gtmlujrmiw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgfzy.top/gtkkvcivdb.html

[R47] sed 单行替换
来源：http://hz.wangshuangyany.cn/gtsqiyfpir.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xinyue.icu/gtfbogtfrv.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtmjivinvv.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtgmiseqzq.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtfpalhakv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtkpmatrua.html

[R50] awk 求和
来源：http://hz.nanxinkj.top/gtfnauujaf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtllhmeafc.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtrqujgqmn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hammf.cn/gtcfblifza.html

[R52] 统计行数
来源：http://hz.snrcjt.cn/gtnnmziroo.html

wc -l a.txt
来源：http://hz.meibo888.top/gtskuijdry.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxuanxn.top/gtleduerml.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhixingplan.top/gtyldegxrp.html

[R54] 比较两个文件
来源：http://hz.jyoumei.cn/gtbmphprko.html

diff a.txt b.txt
来源：http://hz.guannengcc.top/gttjhmafke.html

[R55] 压缩与解压
来源：http://hz.yonumen.top/gtcofjioic.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.snrcjt.cn/gtcjxtoyys.html

[R56] 远程拷贝
来源：http://hz.sufxvd.cn/gtxzxtoxmg.html

scp file user@host:/path/
来源：http://hz.quarkkingdee.top/gtlmrhapzh.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gtqwubexmh.html

ssh user@host 'uptime'
来源：http://hz.gogol.net.cn/gtvxdibgzg.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtqjxwrjxf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daxiang520.top/gtzxdjoxyc.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gttefunwvv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.svipenyu.cn/gthpwbfiyf.html

[R60] 只看 HTTP 状态码
来源：http://hz.gzhubu.top/gtanchxjrj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenlongwang.top/gtjekpwsea.html

[R61] 磁盘占用
来源：http://hz.hammf.cn/gtkmucmdaj.html

df -h;  du -sh *
来源：http://hz.dianchejie.cn/gtsseoucfn.html

[R62] 找最占空间的文件
来源：http://hz.tanke756.top/gtxbsmliap.html

du -ah . | sort -rh | head -10
来源：http://hz.zhiwuduotai.top/gtspfpxcvd.html

[R63] 内存与进程
来源：http://hz.hnqzz.top/gtlgkoqczr.html

free -h;  ps aux | grep nginx
来源：http://hz.xinyue.icu/gtfcsqcnyr.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gtwzfjimtl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgfzy.top/gtlsezlzlf.html

[R65] 查看端口占用
来源：http://hz.xuetiantiany.cn/gttsutfbgn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gtodvxzqes.html

[R66] 定时任务
来源：http://hz.yonumen.top/gtmhsohres.html

crontab -e;  crontab -l
来源：http://hz.yueranfly.top/gtpwuiavzg.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtbbfhaepe.html

openssl rand -hex 16
来源：http://hz.guannengcc.top/gtfqcqzcsm.html

[R68] 计算文件校验值
来源：http://hz.svipenyu.cn/gtxrfjmgxy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cqqwz.cn/gtccqbzppl.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gtuwmwuhdt.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhongyouzk.top/gtmscrsmmu.html

[R70] 时间戳与互转
来源：http://hz.jinqigfzy.top/gtlbvsxlep.html

date +%s;  date -d @1700000000
来源：http://hz.0kj1m.cn/gtqqupywut.html

[R71] 日期格式化
来源：http://hz.nanxinkj.top/gtgdxrtorl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yongpay.top/gttnsolsbr.html

[R72] 等待端口就绪
来源：http://hz.iojbl.cn/gtbveqfdso.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtnmqlgilo.html

[R73] 分割大日志
来源：http://hz.gaohongyu789.top/gtkbftezpx.html

split -l 1000 big.log part_
来源：http://hz.shangyingyoupin.top/gtujtfroit.html

[R74] 批量重命名
来源：http://hz.yj202588.top/gtjzvodwqr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhaomingkeji.xyz/gtgwwyypue.html

[R75] 导出环境变量
来源：http://hz.gzhubu.top/gtxlobeqtf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.vqdsnc.cn/gtfkuwizvs.html

[R76] 使用临时文件
来源：http://hz.havefunace.top/gtjbotasux.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuetiantiany.cn/gtulynqufj.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangkeji.top/gtwyfsstgp.html

read -rp "请输入: " ans
来源：http://hz.fengsongda.top/gtzpbuhnxd.html

[R78] 交互式菜单
来源：http://hz.daria6918.cn/gtkqqisqnx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jiagoushi.top/gtzznlplph.html

[R79] 解析命令行选项
来源：http://hz.guowangkeji.top/gtilnxbmqe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.52xcode.cn/gtnxnmchsh.html

[R80] 查看脚本执行耗时
来源：http://hz.andypj.xyz/gttdaqugtb.html

time ./run.sh
来源：http://hz.tanke756.top/gtgypubkec.html

================================================================================
来源：http://hz.yonumen.top/gtpcgbvbry.html

S. C / C++ 专题
来源：http://hz.zdqjudy.top/gtpoulddzu.html

================================================================================
来源：http://hz.ppjwa.cn/gtwpkrsisv.html

[S01] C：Hello World
来源：http://hz.yj20258888.top/gtqsbbffmh.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gteelgpkkf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fengsongda.top/gtacskgdsw.html

[S02] C：变量与格式化输出
来源：http://hz.shuidangran.top/gtearzslof.html

int a = 10; printf("%d\n", a);
来源：http://hz.havefunace.top/gtcvbslnjj.html

[S03] C：读入整数
来源：http://hz.vqdsnc.cn/gtrtqtcpst.html

int x; scanf("%d", &x);
来源：http://hz.dianchejie.cn/gtwdvrlvmr.html

[S04] C：字符串复制
来源：http://hz.meibo888.top/gtsfwhhgnw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hysaishi.cn/gtjfgnzrie.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtbpanwbfu.html

strlen(s)
来源：http://hz.shanyushiyangkeji.top/gtvyatpqwf.html

[S06] C：字符串比较
来源：http://hz.cqqwz.cn/gtbowxgaod.html

strcmp(a, b) == 0
来源：http://hz.cdnleiting.top/gtvjnutptl.html

[S07] C：数组遍历求和
来源：http://hz.gogol.net.cn/gtoeltwxft.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhongyouzk.top/gtxkdeqsyx.html

[S08] C：动态内存分配与释放
来源：http://hz.316326.xyz/gtacchxlmf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhiwuduotai.top/gtetnmjrie.html

[S09] C：结构体定义与初始化
来源：http://hz.cucudq.cn/gthonkkwof.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daxiang520.top/gtcgeqsncd.html

[S10] C：指针与解引用
来源：http://hz.hywenlv.cn/gtjsfjhlip.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigufen.top/gtwrguxqnz.html

[S11] C：逐行读文件
来源：http://hz.sxryk.cn/gtotioauvx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.andypj.xyz/gtbbfbzlxa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hongshengwenyu.top/gtvcrqsojw.html

fclose(f);
来源：http://hz.zycfv.cn/gtllxsyhme.html

[S12] C：写文件
来源：http://hz.zhixingplan.top/gtyosdzbtc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtphnyerpo.html

[S13] C：宏定义
来源：http://hz.feifeiyinyue.top/gtpldpigtx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hammf.cn/gtmdiqppjx.html

[S14] C：枚举
来源：http://hz.tianlin.xyz/gtogzucrab.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258888.top/gtgptfvpsm.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gtpkpynguv.html

(double) a / b
来源：http://hz.nwbrower.top/gtvyvoxsts.html

[S16] C：位操作置位
来源：http://hz.jiagoushi.top/gtcozfebhn.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtaywocfbt.html

[S17] C：安全拼接字符串
来源：http://hz.jlsjyb.cn/gtgwjtsqec.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhengqikj.top/gtifvcpkvt.html

[S18] C：命令行参数
来源：http://hz.zdqjudy.top/gtijpzimhb.html

int main(int argc, char **argv)
来源：http://hz.ehwqpu.com/gtbknhowvx.html

[S19] C：快速排序
来源：http://hz.0kj1m.cn/gtgxmjplsv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtwjmfxlaj.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtsujzjyip.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.andypj.xyz/gtfpwgtban.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gtzhfhvswt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yuanzhike.top/gtzelheidl.html

[S22] C：字符串转数字
来源：http://hz.sxryk.cn/gtniigszga.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guowangkeji.top/gtgeizkbmz.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtmpmzaqwv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gzhubu.top/gtmarkwsvf.html

[S24] C：获取本地时间
来源：http://hz.tian-w.cn/gtyjreucsv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.mhx1999.top/gtgacemddg.html

[S25] C：内存拷贝
来源：http://hz.hywenlv.cn/gtkufmjdww.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtgqjeunnx.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtwdvpougv.html

memset(a, 0, sizeof a);
来源：http://hz.zhiwuduotai.top/gtuqqywcvn.html

[S27] C：定义常量
来源：http://hz.zhoulong.xyz/gtizirfhet.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtylnznths.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtrynbsiel.html

static int counter = 0;
来源：http://hz.zdqjudy.top/gthumcmcod.html

[S29] C：变参函数
来源：http://hz.shanyushiyangtech.top/gtsvxlhkec.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.feifeiyinyue.top/gtdjlnqzvg.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtomwziuup.html

#ifndef X_H
来源：http://hz.yuanzhike.top/gtxcupmaab.html

#define X_H
来源：http://hz.cheryme.top/gtaxsvhksl.html

#endif
来源：http://hz.chenzaomai.com/gtnbntcyfw.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtvggfvbff.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtprcvaqmr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ivvv.top/gthmmwtdzh.html

[S32] C++：字符串
来源：http://hz.yvedp.cn/gtjepohasx.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtsuagppky.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtayflhmny.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nwbrower.top/gtredmidjk.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtavknhuqm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jlsjyb.cn/gtymlzlkcb.html

[S35] C++：map
来源：http://hz.dianchejie.cn/gtipcgcvdj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gthggbtuns.html

[S36] C++：unordered_map
来源：http://hz.316326.xyz/gtxwzjvuvr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtaqfrhkgz.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtyvcgarel.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jyoumei.cn/gtravtcolv.html

[S38] C++：排序
来源：http://hz.gotoacloud.top/gtglsyhnmj.html

std::sort(v.begin(), v.end());
来源：http://hz.meibo888.top/gtmxpivwoa.html

[S39] C++：自定义比较器排序
来源：http://hz.xuanzx.com/gticuzlrvg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pycfn.com/gtjddpydzy.html

[S40] C++：查找元素
来源：http://hz.gaohongyu789.top/gtlkrtqfyq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.9152youxi.cn/gtptaqqzeh.html

[S41] C++：类与构造函数
来源：http://hz.zhixingplan.top/gtlpcbaiyt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.vqdsnc.cn/gtospnhcpt.html

[S42] C++：继承与虚函数
来源：http://hz.zhaomingkeji.xyz/gtcvxkbqio.html

class B : public Base { public: void f() override {} };
来源：http://hz.jqgfzy.top/gtbgdlbdgw.html

[S43] C++：智能指针
来源：http://hz.9152youxi.cn/gtohwzwiwk.html

auto p = std::make_unique<int>(5);
来源：http://hz.birdmap.top/gtfamleyyx.html

[S44] C++：引用传参
来源：http://hz.haohaochexian.top/gtnagkttmn.html

void inc(int &x) { ++x; }
来源：http://hz.hywenlv.cn/gtxzaactdz.html

[S45] C++：lambda
来源：http://hz.meibo888.top/gtrwcttwly.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zycfv.cn/gttsxyausk.html

[S46] C++：函数模板
来源：http://hz.xinyue.icu/gtyahjmmhq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuanzhike.top/gtfdjkewlm.html

[S47] C++：结构化绑定遍历
来源：http://hz.daria6918.cn/gtunfpvvzd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hysaishi.cn/gtbiqntoob.html

[S48] C++：逐行读文件
来源：http://hz.vqdsnc.cn/gtsdsuxapa.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fengsongda.top/gteawyffoe.html

while (std::getline(in, line)) { }
来源：http://hz.nanxinkj.top/gtzwmooprb.html

[S49] C++：写文件
来源：http://hz.zhongyouzk.top/gthiabsmcd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yanxiufei.cn/gtjsvuhpay.html

[S50] C++：格式化数字
来源：http://hz.gogol.net.cn/gtjylyvofb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.kuanghao11.cn/gteyqlfomh.html

[S51] C++：显式类型转换
来源：http://hz.0kj1m.cn/gttxrwywwu.html

static_cast<double>(a) / b
来源：http://hz.chenlongwang.top/gtxrkijluk.html

[S52] C++：const 与 noexcept
来源：http://hz.gotoacloud.top/gtrkmnvefb.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtfsyxevsp.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtyhujlnvp.html

std::vector<int> w = std::move(v);
来源：http://hz.pycfn.com/gtkevbdnwh.html

[S54] C++：异常处理
来源：http://hz.jianghu66.top/gtiqhdxpch.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pycfn.com/gtlierrmmp.html

[S55] C++：结构化绑定
来源：http://hz.zhiwuduotai.top/gttwwuygwd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ppjwa.cn/gtuwedezjd.html

[S56] C++：optional
来源：http://hz.zhengqikj.top/gtbjfifhbp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jyoumei.cn/gtgqkwednw.html

[S57] C++：编译期常量
来源：http://hz.hammf.cn/gtwfeddhxe.html

constexpr int N = 10;
来源：http://hz.yonumen.top/gtclbimcjj.html

[S58] C++：命名空间
来源：http://hz.guannengcc.top/gtskvuxije.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtdhkejlpy.html

[S59] C++：静态断言
来源：http://hz.shuidangran.top/gtbbdszusf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.0kj1m.cn/gtjfhkyunx.html

[S60] C++：遍历并删除元素
来源：http://hz.svipenyu.cn/gtxfarklwj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gthcxgdfch.html

================================================================================
来源：http://hz.pycfn.com/gtwfabgawq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tanke756.top/gtcggkeeoz.html

================================================================================
来源：http://hz.ybcxt.top/gtktznmeym.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gttkhbfzyu.html

println("Hello")
来源：http://hz.hnxiangtu.top/gtiqsxmsaq.html

[T02] Kotlin：变量
来源：http://hz.jinqigufen.top/gtdoqoilcg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuanzhike.top/gtepnzwefj.html

[T03] Kotlin：字符串模板
来源：http://hz.yuanzhike.top/gtruyvodpz.html

"值: $b"
来源：http://hz.zhongyouzk.top/gtjgafbobr.html

[T04] Kotlin：空安全
来源：http://hz.meibo888.top/gtcpddttsu.html

val n: String? = null;  n?.length
来源：http://hz.yonumen.top/gttksvoydx.html

[T05] Kotlin：when 表达式
来源：http://hz.quarkkingdee.top/gtdbfziahb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tianlin.xyz/gtfqzzyjmb.html

[T06] Kotlin：集合映射
来源：http://hz.meibo888.top/gtgnouqead.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.haohaochexian.top/gtwyxzrovr.html

[T07] Kotlin：集合过滤
来源：http://hz.gogol.net.cn/gttqqhrjvd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.havefunace.top/gtjxuhzbrf.html

[T08] Kotlin：数据类
来源：http://hz.yj20258888.top/gtvzisjlpw.html

data class User(val name: String, val age: Int)
来源：http://hz.meibo888.top/gtktyflyfz.html

[T09] Kotlin：扩展函数
来源：http://hz.bjfxy.top/gtpebxldou.html

fun String.exclaim() = this + "!"
来源：http://hz.andypj.xyz/gtbbltdxqb.html

[T10] Kotlin：默认参数
来源：http://hz.jinyuanbaomall.cn/gtffjrjofy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tian-w.cn/gtexsykjxj.html

[T11] Kotlin：协程
来源：http://hz.nanxinkj.top/gtdrqyedtt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxinkj.top/gtetbrusqv.html

[T12] Kotlin：解构声明
来源：http://hz.yuxming.cn/gtiawvpmia.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtwkvwaklm.html

[T13] Kotlin：只读 Map
来源：http://hz.daxiang520.top/gtjpdssfqn.html

val m = mapOf("a" to 1)
来源：http://hz.ehwqpu.com/gtmsfpmrov.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtdrddzpul.html

for (i in 1..10) println(i)
来源：http://hz.bjfxy.top/gtrcafryxw.html

[T15] Kotlin：接口
来源：http://hz.aizwys.cn/gtzpvucyxy.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtinuoidcn.html

[T16] Swift：Hello World
来源：http://hz.zycfv.cn/gtmigdrxhi.html

print("Hello")
来源：http://hz.gogol.net.cn/gtqtqlkpco.html

[T17] Swift：变量与常量
来源：http://hz.hfpthk.cn/gtxrfdsygy.html

var a = 1;  let b = 2
来源：http://hz.xinyue.icu/gtfrwnymlh.html

[T18] Swift：字符串插值
来源：http://hz.316326.xyz/gtbgrknvck.html

"值: \(b)"
来源：http://hz.xuanzx.com/gtknqyuqqq.html

[T19] Swift：可选绑定
来源：http://hz.bjfxy.top/gtqurqhqvz.html

if let n = opt { print(n) }
来源：http://hz.shanyushiyangkeji.top/gtvklfxudb.html

[T20] Swift：数组操作
来源：http://hz.yj202588.top/gtiyexpqhz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jiagoushi.top/gthtvvbsgg.html

[T21] Swift：遍历
来源：http://hz.cdnleiting.top/gtcdluoicl.html

for x in a { print(x) }
来源：http://hz.hnxiangtu.top/gtydvnqzhc.html

[T22] Swift：字典
来源：http://hz.vqdsnc.cn/gtzcnvwfqx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jiagoushi.top/gtywxeufpd.html

[T23] Swift：函数
来源：http://hz.zycfv.cn/gtlrkkbtna.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xinyue.icu/gtjrnckegc.html

[T24] Swift：闭包
来源：http://hz.zhengqikj.top/gtyfxhigyq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.pycfn.com/gtvdhtqkqz.html

[T25] Swift：结构体
来源：http://hz.shanyushiyangkeji.top/gtsbntfliy.html

struct P { var x: Int }
来源：http://hz.birdmap.top/gtwxfxctsy.html

[T26] Swift：类与重写
来源：http://hz.ivvv.top/gtydqxlsdb.html

class A: Base { override func f() {} }
来源：http://hz.yangfankeji.com/gtbmzqhuyx.html

[T27] Swift：错误处理
来源：http://hz.jyoumei.cn/gtygntuzun.html

do { try f() } catch { print(error) }
来源：http://hz.gzhubu.top/gtfwccspik.html

[T28] Swift：枚举
来源：http://hz.zhengqikj.top/gtxmxrtrjx.html

enum Color { case red, green }
来源：http://hz.shanyushiyangkeji.top/gtorwilbpr.html

[T29] Swift：guard 提前返回
来源：http://hz.zhaomingkeji.xyz/gtooxauzee.html

guard let x = opt else { return }
来源：http://hz.dashuyun.cn/gtoabskfma.html

[T30] Swift：协议
来源：http://hz.cheryme.top/gtrjepahgm.html

protocol Shape { func area() -> Double }
来源：http://hz.chenzaomai.com/gtoilrbmeg.html

[T31] Lua：Hello World
来源：http://hz.snrcjt.cn/gtwfmavmmx.html

print("Hello")
来源：http://hz.yuanzhike.top/gtvnebizmy.html

[T32] Lua：局部变量
来源：http://hz.wangdashe.top/gtqwwnwclr.html

local a = 1
来源：http://hz.hysaishi.cn/gthqnibgoj.html


<!-- 参考信息 -->