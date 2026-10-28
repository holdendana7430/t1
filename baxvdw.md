代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.xingfuxueyuan.xyz/gtfyqakoma.html

[R32] 参数个数校验
来源：http://hz.xziqi.cn/gtqbvlsjju.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtafkzkxjf.html

[R33] 捕获错误并提示行号
来源：http://hz.hnqzz.top/gtxjbwdblg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhijiandao.cn/gtkdjnpffs.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gtyzyvwupq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtytawjuth.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtcfrcknlc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tanke756.top/gtsbxcmbdn.html

[R36] 并发执行多个任务
来源：http://hz.shzxlz.cn/gtvynlduzs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.iojbl.cn/gtwsvsjhbz.html

[R37] 把输出赋给变量
来源：http://hz.yangfankeji.com/gtzfwdxsoi.html

files=$(ls -1)
来源：http://hz.zhaomingkeji.xyz/gtfrksgsbt.html

[R38] 管道串联
来源：http://hz.jinyuanbaomall.cn/gtwbwptuho.html

cat a.txt | grep -i error | wc -l
来源：http://hz.52xcode.cn/gtqznexxfe.html

[R39] 重定向标准输出与错误
来源：http://hz.wangshuangyany.cn/gtrgssmpor.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtzkkdrybc.html

[R40] 追加写日志
来源：http://hz.andypj.xyz/gtpmstkzdd.html

echo "log" >> out.log
来源：http://hz.zhoulong.xyz/gtjfpjsots.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtxwalbdxl.html

cmd >/dev/null 2>&1
来源：http://hz.zhongyouzk.top/gtuyitlgqo.html

[R42] 输入重定向
来源：http://hz.c1oappe.top/gtznyzjczh.html

wc -l < a.txt
来源：http://hz.birdmap.top/gteqtrjvux.html

[R43] 按名字查找文件
来源：http://hz.cdnleiting.top/gttyquvmdl.html

find . -name "*.log" -type f
来源：http://hz.mhx1999.top/gtzmrvfmia.html

[R44] 按修改时间查找
来源：http://hz.hammf.cn/gtrddsppvm.html

find . -mtime -7 -type f
来源：http://hz.yj20258888.top/gtkxzeyolu.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtkmipgftl.html

find . -name "*.tmp" -delete
来源：http://hz.andypj.xyz/gtbmpzdjha.html

[R46] 递归替换文件内容
来源：http://hz.yonumen.top/gtxhtdhwjh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hywenlv.cn/gtvggovccl.html

[R47] sed 单行替换
来源：http://hz.zhijiandao.cn/gtnvyldgnz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.c1oappe.top/gtgsxnhdan.html

[R48] awk 取指定列
来源：http://hz.ybcxt.top/gtesthqnwh.html

awk '{print $1, $3}' a.txt
来源：http://hz.aizwys.cn/gttkemdhyo.html

[R49] awk 带条件
来源：http://hz.zhengqikj.top/gtrllydtfg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pycfn.com/gtvesjncmf.html

[R50] awk 求和
来源：http://hz.shanyushiyangtech.top/gtzqhkpyoh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nwbrower.top/gtgkdxxdlo.html

[R51] 排序去重取前几
来源：http://hz.andypj.xyz/gtcmazyvav.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shangyingyoupin.top/gtzdoqgwng.html

[R52] 统计行数
来源：http://hz.pycfn.com/gtkdshioeq.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtdtlmtnvt.html

[R53] 查看文件头与实时尾
来源：http://hz.zdqjudy.top/gthtepqeca.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shzxlz.cn/gtlktnwpmm.html

[R54] 比较两个文件
来源：http://hz.smart0.xyz/gtgjcyizwj.html

diff a.txt b.txt
来源：http://hz.shanyushiyangtech.top/gtiavuxegi.html

[R55] 压缩与解压
来源：http://hz.haohaochexian.top/gtypnfcici.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sysykeji.top/gtahtyhdoc.html

[R56] 远程拷贝
来源：http://hz.cheryme.top/gtcujrgade.html

scp file user@host:/path/
来源：http://hz.hysaishi.cn/gtknxjgtmz.html

[R57] 远程执行命令
来源：http://hz.hnxiangtu.top/gtxhnheyez.html

ssh user@host 'uptime'
来源：http://hz.hammf.cn/gtocjckvqk.html

[R58] 下载文件
来源：http://hz.cdnleiting.top/gtacermxdt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtuxmcvxvj.html

[R59] 发 POST JSON
来源：http://hz.hnxiangtu.top/gtctutqnme.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gtbbvosyiu.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtzvuzlaww.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yvedp.cn/gtjelzcbfe.html

[R61] 磁盘占用
来源：http://hz.hywenlv.cn/gtfnjsveuw.html

df -h;  du -sh *
来源：http://hz.gogol.net.cn/gtlnzudiug.html

[R62] 找最占空间的文件
来源：http://hz.shangyingyoupin.top/gtldirlipe.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtpkjtzvcm.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtsswnziwg.html

free -h;  ps aux | grep nginx
来源：http://hz.chenlongwang.top/gtluntmreb.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtibwccbup.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hammf.cn/gtyhxlgyac.html

[R65] 查看端口占用
来源：http://hz.ydzc1.top/gtfpsyjjup.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hongshengwenyu.top/gtyhfovacd.html

[R66] 定时任务
来源：http://hz.chenlongwang.top/gtspsiornm.html

crontab -e;  crontab -l
来源：http://hz.cheryme.top/gtyynzehhr.html

[R67] 生成随机十六进制串
来源：http://hz.meibo888.top/gtkgdjbxzh.html

openssl rand -hex 16
来源：http://hz.yj202588.top/gtqgjetbip.html

[R68] 计算文件校验值
来源：http://hz.tanke756.top/gtcenjxdnz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtinjzgcmd.html

[R69] 生成随机密码
来源：http://hz.hfpthk.cn/gteicowrbq.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenlongwang.top/gtdvaavzfq.html

[R70] 时间戳与互转
来源：http://hz.gaohongyu789.top/gtgyurlcha.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtsrklytuq.html

[R71] 日期格式化
来源：http://hz.pengpengdd.cyou/gtykssbuxe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydzc1.top/gtgwezonzz.html

[R72] 等待端口就绪
来源：http://hz.zdqjudy.top/gtjhcstjyf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xinyue.icu/gtqwgeoibx.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtvgdtpekf.html

split -l 1000 big.log part_
来源：http://hz.daxiang520.top/gtyviapmuy.html

[R74] 批量重命名
来源：http://hz.nwbrower.top/gtxlysbsnb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zdqjudy.top/gtywkzpzgy.html

[R75] 导出环境变量
来源：http://hz.yuanzhike.top/gtsohdxjwd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtgkxxvkja.html

[R76] 使用临时文件
来源：http://hz.snrcjt.cn/gtkncyqbjg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.fzhhl.top/gttqzuxazd.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtcqnhtzxh.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtujswqluk.html

[R78] 交互式菜单
来源：http://hz.yj20258888.top/gtfmckrlog.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hywenlv.cn/gtcposbydh.html

[R79] 解析命令行选项
来源：http://hz.jinghuilouyu.cn/gtxwzspnrh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtxhujcryp.html

[R80] 查看脚本执行耗时
来源：http://hz.hfpthk.cn/gtbrjodcvi.html

time ./run.sh
来源：http://hz.daria6918.cn/gtvrgkbyes.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtoipnrjke.html

S. C / C++ 专题
来源：http://hz.xuetiantiany.cn/gtrwtfsunj.html

================================================================================
来源：http://hz.bjfxy.top/gtxpbprgvj.html

[S01] C：Hello World
来源：http://hz.hammf.cn/gtqcqdgoew.html

#include <stdio.h>
来源：http://hz.jinqigufen.top/gteaxvypof.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hywenlv.cn/gtxivhaxss.html

[S02] C：变量与格式化输出
来源：http://hz.zhengqikj.top/gtxdoyvjlh.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhoulong.xyz/gtopkexfke.html

[S03] C：读入整数
来源：http://hz.yj20258888.top/gtkuqrwclq.html

int x; scanf("%d", &x);
来源：http://hz.xuetiantiany.cn/gtypuhhyib.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gteyjwzgco.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.aizwys.cn/gthhiaokiw.html

[S05] C：字符串长度
来源：http://hz.yangfankeji.com/gtdjhjvsuy.html

strlen(s)
来源：http://hz.mhx1999.top/gtfkqupmqb.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtfecavzto.html

strcmp(a, b) == 0
来源：http://hz.wangshuangyany.cn/gtpvtpytqv.html

[S07] C：数组遍历求和
来源：http://hz.redwolf501.top/gtkujslwby.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenjidiqi.icu/gtmthvnqhf.html

[S08] C：动态内存分配与释放
来源：http://hz.yueranfly.top/gthtprrjvi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gaohongyu789.top/gtyewfkswh.html

[S09] C：结构体定义与初始化
来源：http://hz.0kj1m.cn/gttuipmgsf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guannengcc.top/gtqimqbqci.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangkeji.top/gtxsbjjdwi.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigfzy.top/gtbzmsdugm.html

[S11] C：逐行读文件
来源：http://hz.smart0.xyz/gtpqtrwyxn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnqzz.top/gtwyxhxxql.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgfzy.top/gtoqbqyxkp.html

fclose(f);
来源：http://hz.andypj.xyz/gtweywufjx.html

[S12] C：写文件
来源：http://hz.bjfxy.top/gtdxdbueou.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtixewhcfq.html

[S13] C：宏定义
来源：http://hz.mhx1999.top/gtumiqtnyz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtdakrjnsm.html

[S14] C：枚举
来源：http://hz.cdnleiting.top/gtayskkmoa.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shangyingyoupin.top/gtrsfhvotm.html

[S15] C：类型转换
来源：http://hz.xuetiantiany.cn/gtxbetlbar.html

(double) a / b
来源：http://hz.redwolf501.top/gtavolbccx.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gtofzdxvvw.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gteowkeytg.html

[S17] C：安全拼接字符串
来源：http://hz.hywenlv.cn/gtqaedtslo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gzhubu.top/gtnfjxslfw.html

[S18] C：命令行参数
来源：http://hz.hnxiangtu.top/gtllqvefmn.html

int main(int argc, char **argv)
来源：http://hz.snrcjt.cn/gthqisanfv.html

[S19] C：快速排序
来源：http://hz.zhixingplan.top/gtnnquhcjx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtcjyprqvj.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtdgstyojo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtlzrmwone.html

[S21] C：字符类别判断
来源：http://hz.tian-w.cn/gtnwkbolnq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tian-w.cn/gturqznzpt.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gteoazkymi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tanke756.top/gtjejjnywx.html

[S23] C：随机数
来源：http://hz.hammf.cn/gtqhawylov.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhijiandao.cn/gtkanexxqu.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gtmxcyaegz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yanxiufei.cn/gtvwtmlhvv.html

[S25] C：内存拷贝
来源：http://hz.aibaodan.cn/gtthzfgqij.html

memcpy(dst, src, n);
来源：http://hz.guowangkeji.top/gtknafrsou.html

[S26] C：内存清零
来源：http://hz.haohaochexian.top/gtheqjvkhf.html

memset(a, 0, sizeof a);
来源：http://hz.yueranfly.top/gtcnoswagh.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtefppngvp.html

const double PI = 3.14159;
来源：http://hz.xylfe.cn/gtmgcvfhcw.html

[S28] C：静态变量
来源：http://hz.hammf.cn/gttgpjjfgu.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtfkrhqlwu.html

[S29] C：变参函数
来源：http://hz.cdnleiting.top/gtnnbhutih.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gtasjbhamr.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtxvfwowru.html

#ifndef X_H
来源：http://hz.xinyue.icu/gttovvxccp.html

#define X_H
来源：http://hz.shzxlz.cn/gtyszouumt.html

#endif
来源：http://hz.hnqzz.top/gtlmltxlyb.html

[S31] C++：Hello World
来源：http://hz.wangshuangyany.cn/gtoawvkmcy.html

#include <iostream>
来源：http://hz.zhongyouzk.top/gtvupfexfk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gtytplbklt.html

[S32] C++：字符串
来源：http://hz.hnxiangtu.top/gtspwfmdpd.html

std::string s = "hi";  s += "!";
来源：http://hz.zhixingplan.top/gtrehwgiml.html

[S33] C++：vector 增删
来源：http://hz.daria6918.cn/gtsnxtyeoe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hnxiangtu.top/gtwlbsofmy.html

[S34] C++：遍历 vector
来源：http://hz.chenlongwang.top/gtclqmtjjj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xylfe.cn/gtftfdblzt.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtprgtomrz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtxnjashdg.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gtjnhbpcrq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtxsroajjf.html

[S37] C++：set
来源：http://hz.cdnleiting.top/gttsmqbgej.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gtdrjegazz.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtflfhfetn.html

std::sort(v.begin(), v.end());
来源：http://hz.jlsjyb.cn/gtpyijspbw.html

[S39] C++：自定义比较器排序
来源：http://hz.ydjk.org.cn/gtgpqkxidr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.snrcjt.cn/gthkyxbriq.html

[S40] C++：查找元素
来源：http://hz.zhixingplan.top/gtbyophxax.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigufen.top/gtuqngnych.html

[S41] C++：类与构造函数
来源：http://hz.yanxiufei.cn/gttvjzlksk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenjidiqi.icu/gtsjbtpfvj.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtlpwrygtu.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gtmvjbhsub.html

[S43] C++：智能指针
来源：http://hz.sysykeji.top/gtfgohnxtf.html

auto p = std::make_unique<int>(5);
来源：http://hz.vqdsnc.cn/gtxsvojuua.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtmdpqjtiq.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigfzy.top/gtdriojzat.html

[S45] C++：lambda
来源：http://hz.cheryme.top/gtjnnajefy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.smart0.xyz/gtitomvccj.html

[S46] C++：函数模板
来源：http://hz.andypj.xyz/gtyagpdypc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgufenzy.top/gtmmphmbhm.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtivvkeuxp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gtckrggswy.html

[S48] C++：逐行读文件
来源：http://hz.hammf.cn/gtgesnhxel.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ywan-chungtsiang.top/gtwzfyyuwz.html

while (std::getline(in, line)) { }
来源：http://hz.yuxming.cn/gtyqknaxvt.html

[S49] C++：写文件
来源：http://hz.jinqigufen.top/gtzdvicvqa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydzc1.top/gtazwsmhif.html

[S50] C++：格式化数字
来源：http://hz.jinghuilouyu.cn/gtecyzkdws.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gotoacloud.top/gtbkcjbmgn.html

[S51] C++：显式类型转换
来源：http://hz.sysykeji.top/gtkmgphhsz.html

static_cast<double>(a) / b
来源：http://hz.xinyue.icu/gtfarjlmxa.html

[S52] C++：const 与 noexcept
来源：http://hz.ybcxt.top/gtubcjrkuh.html

int size() const noexcept { return n_; }
来源：http://hz.tian-w.cn/gtduvmqphi.html

[S53] C++：移动语义
来源：http://hz.andypj.xyz/gtbozjrkhb.html

std::vector<int> w = std::move(v);
来源：http://hz.xuanzx.com/gtwesdmhos.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gtaepqqwir.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tian-w.cn/gtkybuwkhk.html

[S55] C++：结构化绑定
来源：http://hz.havefunace.top/gtisljntvn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ybcxt.top/gtdcmmdpjd.html

[S56] C++：optional
来源：http://hz.jqgfzy.top/gtrikglkaw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinyuanbaomall.cn/gtyueaxnfk.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gtyahayjok.html

constexpr int N = 10;
来源：http://hz.zhixingplan.top/gtacrnvbtm.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gthwbrljft.html

namespace ns { int f() { return 1; } }
来源：http://hz.svipenyu.cn/gtunizkeyd.html

[S59] C++：静态断言
来源：http://hz.vqdsnc.cn/gtejqnajzo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jlsjyb.cn/gtkbccnnxt.html

[S60] C++：遍历并删除元素
来源：http://hz.andypj.xyz/gtldfcqfun.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gogol.net.cn/gtkdnpcuwb.html

================================================================================
来源：http://hz.gogol.net.cn/gtklkwttua.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.haohaochexian.top/gtuhtypzvq.html

================================================================================
来源：http://hz.hammf.cn/gtlfsaitgu.html

[T01] Kotlin：Hello World
来源：http://hz.hammf.cn/gtxnsbdlaf.html

println("Hello")
来源：http://hz.ppjwa.cn/gteceeojzu.html

[T02] Kotlin：变量
来源：http://hz.ppjwa.cn/gtdpnqwybv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.dashuyun.cn/gtvuinmtqt.html

[T03] Kotlin：字符串模板
来源：http://hz.xylfe.cn/gtswfsundg.html

"值: $b"
来源：http://hz.jinyuanbaomall.cn/gthoesghgh.html

[T04] Kotlin：空安全
来源：http://hz.sysykeji.top/gtmfemvscq.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtcozvqqbh.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtxomxsfus.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xziqi.cn/gtjhvgixux.html

[T06] Kotlin：集合映射
来源：http://hz.nanxinkj.top/gtwgeratwf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydzc1.top/gtvvukjroz.html

[T07] Kotlin：集合过滤
来源：http://hz.jiagoushi.top/gtdcwupumt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnxiangtu.top/gtqgtbrilb.html

[T08] Kotlin：数据类
来源：http://hz.ydzc1.top/gtcoclnhxc.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtshxtlpsb.html

[T09] Kotlin：扩展函数
来源：http://hz.gzhubu.top/gtlnozcsmy.html

fun String.exclaim() = this + "!"
来源：http://hz.yangfankeji.com/gtmpgbafeu.html

[T10] Kotlin：默认参数
来源：http://hz.cqqwz.cn/gttznprbvd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.havefunace.top/gtvbntbogh.html

[T11] Kotlin：协程
来源：http://hz.nwbrower.top/gttcmytthk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yonumen.top/gtvbtnglrr.html

[T12] Kotlin：解构声明
来源：http://hz.c1oappe.top/gtlxcnxkor.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinqigufen.top/gtaybrgybz.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gtakoddsna.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gtmdkflxhj.html

[T14] Kotlin：循环
来源：http://hz.cheryme.top/gtcirsvqcf.html

for (i in 1..10) println(i)
来源：http://hz.zhijiandao.cn/gthhnkcpej.html

[T15] Kotlin：接口
来源：http://hz.jinqigfzy.top/gtkfivqris.html

interface Shape { fun area(): Double }
来源：http://hz.52xcode.cn/gtditcfngx.html

[T16] Swift：Hello World
来源：http://hz.cashguo.top/gtffvkauxx.html

print("Hello")
来源：http://hz.smart0.xyz/gtdlnxubzj.html

[T17] Swift：变量与常量
来源：http://hz.gogol.net.cn/gtkyhgpfqg.html

var a = 1;  let b = 2
来源：http://hz.316326.xyz/gtzoiazwto.html

[T18] Swift：字符串插值
来源：http://hz.zhijiandao.cn/gtkazppqyr.html

"值: \(b)"
来源：http://hz.hfpthk.cn/gtoncqfnke.html

[T19] Swift：可选绑定
来源：http://hz.haohaochexian.top/gtpsktstfo.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gtwlhrwebd.html

[T20] Swift：数组操作
来源：http://hz.zhijiandao.cn/gtxelvjxfm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gaohongyu789.top/gtnmprvjgt.html

[T21] Swift：遍历
来源：http://hz.yj20258.top/gtjjrrovzy.html

for x in a { print(x) }
来源：http://hz.iojbl.cn/gtlgiqsavw.html

[T22] Swift：字典
来源：http://hz.xuanzx.com/gtbukzsvpv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtmuvcxrxd.html

[T23] Swift：函数
来源：http://hz.nwbrower.top/gtezqmtpun.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zdqjudy.top/gtrassszwj.html

[T24] Swift：闭包
来源：http://hz.chenzaomai.com/gtnxqcnepk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenjidiqi.icu/gtiiwsehfd.html

[T25] Swift：结构体
来源：http://hz.yj20258888.top/gtzpgfefdn.html

struct P { var x: Int }
来源：http://hz.shanyushiyangkeji.top/gtrsaoxkbg.html

[T26] Swift：类与重写
来源：http://hz.sweek.top/gtapqvgwed.html

class A: Base { override func f() {} }
来源：http://hz.gaohongyu789.top/gtjxjscqem.html

[T27] Swift：错误处理
来源：http://hz.shanyushiyangkeji.top/gtmhlabgzk.html

do { try f() } catch { print(error) }
来源：http://hz.xylfe.cn/gtsmqleqkf.html

[T28] Swift：枚举
来源：http://hz.gaohongyu789.top/gtrdkpmuna.html

enum Color { case red, green }
来源：http://hz.quarkkingdee.top/gtdswbasus.html

[T29] Swift：guard 提前返回
来源：http://hz.zhongyouzk.top/gtiqyugnbq.html

guard let x = opt else { return }
来源：http://hz.9152youxi.cn/gtutsjuryh.html

[T30] Swift：协议
来源：http://hz.daria6918.cn/gtrvxqlvur.html

protocol Shape { func area() -> Double }
来源：http://hz.pycfn.com/gtpftugdiq.html

[T31] Lua：Hello World
来源：http://hz.jlsjyb.cn/gtpjfvntax.html

print("Hello")
来源：http://hz.yonumen.top/gtdiatybmn.html

[T32] Lua：局部变量
来源：http://hz.aizwys.cn/gtybmrtvtt.html

local a = 1
来源：http://hz.9152youxi.cn/gtzgehdonv.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gtsbjzalso.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangshuangyany.cn/gtaopnsmkm.html

[T34] Lua：遍历表
来源：http://hz.jqgfzy.top/gtoqivioqv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.dashuyun.cn/gtundpjwdp.html


<!-- 参考信息 -->