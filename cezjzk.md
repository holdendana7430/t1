代发 wailian999

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtslyvyfyj.html

[R28] 浮点运算
来源：http://hz.vqdsnc.cn/gtkpodhczz.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtxsfjfsfq.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtgjblvzov.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.bjfxy.top/gtnevcrqie.html

[R30] 函数返回状态码
来源：http://hz.sweek.top/gtcfvvtcqo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cqqwz.cn/gtkdmlyjwf.html

[R31] 局部变量
来源：http://hz.wangdashe.top/gtapcakwkc.html

f() { local x=1; echo "$x"; }
来源：http://hz.nwbrower.top/gtalemlqxi.html

[R32] 参数个数校验
来源：http://hz.yueranfly.top/gttbaugsoj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ehwqpu.com/gtqvtefjyh.html

[R33] 捕获错误并提示行号
来源：http://hz.hysaishi.cn/gtvbrxqlwa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.kuanghao11.cn/gtntqhmssa.html

[R34] 退出时清理
来源：http://hz.havefunace.top/gtyujeszgo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtvckrnyuz.html

[R35] 后台执行并等待
来源：http://hz.nanxinkj.top/gttvwabnkn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtmvdlxfxg.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gtrqqhmqwg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhaomingkeji.xyz/gthhphghud.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtjjnplwyn.html

files=$(ls -1)
来源：http://hz.sysykeji.top/gtkwdedger.html

[R38] 管道串联
来源：http://hz.smart0.xyz/gtcpbwljxz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtgrkmuqcf.html

[R39] 重定向标准输出与错误
来源：http://hz.meibo888.top/gtbagzahak.html

cmd > out.log 2>&1
来源：http://hz.hnxiangtu.top/gtwiacbtzk.html

[R40] 追加写日志
来源：http://hz.0kj1m.cn/gtlultuecv.html

echo "log" >> out.log
来源：http://hz.zhongyouzk.top/gtagfkvhwd.html

[R41] 丢弃输出
来源：http://hz.9152youxi.cn/gtanskrhaw.html

cmd >/dev/null 2>&1
来源：http://hz.cucudq.cn/gtkjdwqkup.html

[R42] 输入重定向
来源：http://hz.jiagoushi.top/gthqkjoozb.html

wc -l < a.txt
来源：http://hz.gotoacloud.top/gtrjbqngtc.html

[R43] 按名字查找文件
来源：http://hz.zdqjudy.top/gtgjbwjxcg.html

find . -name "*.log" -type f
来源：http://hz.hongshengwenyu.top/gtiuojjhwa.html

[R44] 按修改时间查找
来源：http://hz.birdmap.top/gtryikvpsb.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtqcizxpox.html

[R45] 批量删除
来源：http://hz.yuxming.cn/gtoeyxpkyu.html

find . -name "*.tmp" -delete
来源：http://hz.daxiang520.top/gtagfmdmxo.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gtbqewqzys.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.kuanghao11.cn/gttjpumhmb.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gtqouxylqv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuanzx.com/gtvktfwwtm.html

[R48] awk 取指定列
来源：http://hz.shuidangran.top/gtjgqbmawq.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj202588.top/gtcndalxqg.html

[R49] awk 带条件
来源：http://hz.xziqi.cn/gtxjdcctqn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtfemcepgj.html

[R50] awk 求和
来源：http://hz.0kj1m.cn/gtcusfcgcs.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnxiangtu.top/gtchbmewja.html

[R51] 排序去重取前几
来源：http://hz.vqdsnc.cn/gteycyuixz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.kuanghao11.cn/gtbavfygwk.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtwrnhnhhi.html

wc -l a.txt
来源：http://hz.smart0.xyz/gtdqtfjdjm.html

[R53] 查看文件头与实时尾
来源：http://hz.redwolf501.top/gtayjgohvi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinyuanbaomall.cn/gtsynliptz.html

[R54] 比较两个文件
来源：http://hz.bjfxy.top/gtschtjoim.html

diff a.txt b.txt
来源：http://hz.yongpay.top/gthwffxvwa.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gthifidvrp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnqzz.top/gtbqxulomn.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtdcpeasuy.html

scp file user@host:/path/
来源：http://hz.xuetiantiany.cn/gtyxpmmeyd.html

[R57] 远程执行命令
来源：http://hz.yangfankeji.com/gtzuycjkaa.html

ssh user@host 'uptime'
来源：http://hz.jinqigufen.top/gtqimovxoc.html

[R58] 下载文件
来源：http://hz.sysykeji.top/gtknyjzbzc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sysykeji.top/gtsvzfjkpy.html

[R59] 发 POST JSON
来源：http://hz.dashuyun.cn/gtajnykuym.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtscvxuqza.html

[R60] 只看 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtgafojesc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yueranfly.top/gtpshkubeb.html

[R61] 磁盘占用
来源：http://hz.tianlin.xyz/gtcitwfzjv.html

df -h;  du -sh *
来源：http://hz.sxryk.cn/gthxxoyrbt.html

[R62] 找最占空间的文件
来源：http://hz.kuanghao11.cn/gtjumanrgt.html

du -ah . | sort -rh | head -10
来源：http://hz.jinqigufen.top/gtcoodugyt.html

[R63] 内存与进程
来源：http://hz.shuidangran.top/gticnliwww.html

free -h;  ps aux | grep nginx
来源：http://hz.tianlin.xyz/gtjwkcbxfv.html

[R64] 结束进程
来源：http://hz.ppjwa.cn/gtzowhrzpd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtdilbqsuo.html

[R65] 查看端口占用
来源：http://hz.nanxuanxn.top/gtyglejldp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shangyingyoupin.top/gtowxflvrg.html

[R66] 定时任务
来源：http://hz.aizwys.cn/gtlaykplxc.html

crontab -e;  crontab -l
来源：http://hz.jinyuanbaomall.cn/gtujnmudfd.html

[R67] 生成随机十六进制串
来源：http://hz.snrcjt.cn/gtvlrbzqjy.html

openssl rand -hex 16
来源：http://hz.hnqzz.top/gtvfxhqyrm.html

[R68] 计算文件校验值
来源：http://hz.quarkkingdee.top/gtdtwryire.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgufenzy.top/gtwqvyipvp.html

[R69] 生成随机密码
来源：http://hz.xingfuxueyuan.xyz/gtomiyyayh.html

head -c 16 /dev/urandom | base64
来源：http://hz.zdqjudy.top/gtghetjkgk.html

[R70] 时间戳与互转
来源：http://hz.kuanghao11.cn/gtvkcqhcsa.html

date +%s;  date -d @1700000000
来源：http://hz.meibo888.top/gtphdzpogo.html

[R71] 日期格式化
来源：http://hz.cdnleiting.top/gtmcoqkilp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnqzz.top/gtqzojkfmd.html

[R72] 等待端口就绪
来源：http://hz.yanxiufei.cn/gtspsxryny.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.meibo888.top/gtrmrztezs.html

[R73] 分割大日志
来源：http://hz.meibo888.top/gtwbiwmuib.html

split -l 1000 big.log part_
来源：http://hz.hnqzz.top/gtzekjpldj.html

[R74] 批量重命名
来源：http://hz.dianchejie.cn/gtbzvmjnqr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yangfankeji.com/gtyuhngxzn.html

[R75] 导出环境变量
来源：http://hz.yanxiufei.cn/gtiexlzwve.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gtjwucwwic.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtzhdjgktj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtkxjrhttf.html

[R77] 读取用户输入
来源：http://hz.gzhubu.top/gtcknoiiha.html

read -rp "请输入: " ans
来源：http://hz.yj20258.top/gtcpruqrkf.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtivphqyoa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.vqdsnc.cn/gtzkgzwkrv.html

[R79] 解析命令行选项
来源：http://hz.aibaodan.cn/gtsdjegbzz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tian-w.cn/gtptufsrnr.html

[R80] 查看脚本执行耗时
来源：http://hz.c1oappe.top/gtbsbhpllv.html

time ./run.sh
来源：http://hz.ybcxt.top/gtrrjqtkoj.html

================================================================================
来源：http://hz.cqqwz.cn/gthdfgxtvi.html

S. C / C++ 专题
来源：http://hz.hnxiangtu.top/gtmgqyfvlv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtlszvusxa.html

[S01] C：Hello World
来源：http://hz.yj20258888.top/gtwyecagjj.html

#include <stdio.h>
来源：http://hz.tianlin.xyz/gtclamgplc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxuanxn.top/gtdsmihslj.html

[S02] C：变量与格式化输出
来源：http://hz.sysykeji.top/gtcxiiutyc.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258888.top/gtjqsbmzdi.html

[S03] C：读入整数
来源：http://hz.jiagoushi.top/gtpyshwzew.html

int x; scanf("%d", &x);
来源：http://hz.andypj.xyz/gtxspwgnha.html

[S04] C：字符串复制
来源：http://hz.jinghuilouyu.cn/gtgxylytgc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnxiangtu.top/gtszwhpykl.html

[S05] C：字符串长度
来源：http://hz.cucudq.cn/gtjfwzoutk.html

strlen(s)
来源：http://hz.sweek.top/gtlnwazehl.html

[S06] C：字符串比较
来源：http://hz.zhengqikj.top/gtwlxlyuuw.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gtwkhyipvv.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtgwbhdmuw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.havefunace.top/gtdrjksrzw.html

[S08] C：动态内存分配与释放
来源：http://hz.zhiwuduotai.top/gtpjjxrezg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtsvvdcsqv.html

[S09] C：结构体定义与初始化
来源：http://hz.shanyushiyangkeji.top/gtarzctlzi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jlsjyb.cn/gtszmahqis.html

[S10] C：指针与解引用
来源：http://hz.sysykeji.top/gtmrluyjea.html

int *p = &a;  *p = 5;
来源：http://hz.zhiwuduotai.top/gtvpxktnzr.html

[S11] C：逐行读文件
来源：http://hz.cucudq.cn/gtqthjirgk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhixingplan.top/gtnkprwstd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gtiuchsntv.html

fclose(f);
来源：http://hz.kuanghao11.cn/gtdvhkotqm.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gtimqhnmtv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gthloigmgs.html

[S13] C：宏定义
来源：http://hz.xuetiantiany.cn/gtrqqtyrva.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258.top/gtijyyelbg.html

[S14] C：枚举
来源：http://hz.shangyingyoupin.top/gtaektrjnr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shzxlz.cn/gtrkqzkdnw.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtdapyyoeb.html

(double) a / b
来源：http://hz.tanke756.top/gtwiidhnhf.html

[S16] C：位操作置位
来源：http://hz.jinqigfzy.top/gtrwgbmhka.html

x |= (1 << 3);
来源：http://hz.jinqigufen.top/gthmylkxdx.html

[S17] C：安全拼接字符串
来源：http://hz.jiagoushi.top/gtfnpwrinm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yongpay.top/gtzudrfgas.html

[S18] C：命令行参数
来源：http://hz.9152youxi.cn/gtdpffmqbs.html

int main(int argc, char **argv)
来源：http://hz.jinqigufen.top/gtyrlnwhpo.html

[S19] C：快速排序
来源：http://hz.xingfuxueyuan.xyz/gtbmlylees.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtwdubxvis.html

[S20] C：二分查找
来源：http://hz.snrcjt.cn/gtqjnqxebu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtmuhugbtg.html

[S21] C：字符类别判断
来源：http://hz.kuanghao11.cn/gtqboqlpyj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ppjwa.cn/gtxellnhuj.html

[S22] C：字符串转数字
来源：http://hz.hammf.cn/gtjcuyffrv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.birdmap.top/gtrpwtwpsy.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gtwqvaawrv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtxzadddmk.html

[S24] C：获取本地时间
来源：http://hz.yueranfly.top/gtkcrofqdm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigfzy.top/gtzwpvvpac.html

[S25] C：内存拷贝
来源：http://hz.shzxlz.cn/gtibautqho.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtvsxgdvhp.html

[S26] C：内存清零
来源：http://hz.9152youxi.cn/gtykjbcess.html

memset(a, 0, sizeof a);
来源：http://hz.xinyue.icu/gtxgplhuyv.html

[S27] C：定义常量
来源：http://hz.yj202588.top/gtunepmuww.html

const double PI = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtvnednauf.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtyldjyhbd.html

static int counter = 0;
来源：http://hz.zhixingplan.top/gtozftzhbc.html

[S29] C：变参函数
来源：http://hz.xingfuxueyuan.xyz/gtdvwifsva.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gthibfyrar.html

[S30] C：头文件保护
来源：http://hz.chenzaomai.com/gtmdysoqxw.html

#ifndef X_H
来源：http://hz.hammf.cn/gtnhirfyev.html

#define X_H
来源：http://hz.yj20258888.top/gthnfhjqcn.html

#endif
来源：http://hz.xinyue.icu/gtwhxtpbve.html

[S31] C++：Hello World
来源：http://hz.yvedp.cn/gtrtwieemc.html

#include <iostream>
来源：http://hz.cdnleiting.top/gtawjbmdpv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhijiandao.cn/gtmvsnhugi.html

[S32] C++：字符串
来源：http://hz.hywenlv.cn/gtowxstdtt.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gthhmwmqed.html

[S33] C++：vector 增删
来源：http://hz.hfpthk.cn/gtbdmmhler.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhijiandao.cn/gtuskahyfe.html

[S34] C++：遍历 vector
来源：http://hz.ivvv.top/gtquivjnxi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gtijvuszpa.html

[S35] C++：map
来源：http://hz.0kj1m.cn/gtrrzwiohx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtloveexuh.html

[S36] C++：unordered_map
来源：http://hz.jinqigufen.top/gtswundgwf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtjzukkrwh.html

[S37] C++：set
来源：http://hz.svipenyu.cn/gtiikoqcpu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuanzhike.top/gtgdpatzqw.html

[S38] C++：排序
来源：http://hz.sysykeji.top/gtnpmcgxqu.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtidnrlije.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtyzxckvef.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangkeji.top/gtuhwxhicg.html

[S40] C++：查找元素
来源：http://hz.jiagoushi.top/gtpgkdopej.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtvnkazzby.html

[S41] C++：类与构造函数
来源：http://hz.yuanzhike.top/gtsmqvvvtv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.fengsongda.top/gtwejrtiof.html

[S42] C++：继承与虚函数
来源：http://hz.hfpthk.cn/gttbqotvmy.html

class B : public Base { public: void f() override {} };
来源：http://hz.mhx1999.top/gtjbykgzhw.html

[S43] C++：智能指针
来源：http://hz.jinqigufen.top/gtlkhmkhrc.html

auto p = std::make_unique<int>(5);
来源：http://hz.snrcjt.cn/gtmhdiunnv.html

[S44] C++：引用传参
来源：http://hz.ehwqpu.com/gtvniltpcz.html

void inc(int &x) { ++x; }
来源：http://hz.andypj.xyz/gtocpyuzjl.html

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtqzkijutu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhoulong.xyz/gtunpgonhs.html

[S46] C++：函数模板
来源：http://hz.yvedp.cn/gtyjiuqcol.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.iojbl.cn/gtffjawfmx.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gtfemxgpzo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cheryme.top/gtempdyehv.html

[S48] C++：逐行读文件
来源：http://hz.yuxming.cn/gtijrorumu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtgwmntvry.html

while (std::getline(in, line)) { }
来源：http://hz.dashuyun.cn/gtveaikwfz.html

[S49] C++：写文件
来源：http://hz.ybcxt.top/gtdqwucfcx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guowangkeji.top/gtjmonrrpg.html

[S50] C++：格式化数字
来源：http://hz.shzxlz.cn/gtnowlxgzr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ivvv.top/gtvlxxycbi.html

[S51] C++：显式类型转换
来源：http://hz.jqgufenzy.top/gtputgqglq.html

static_cast<double>(a) / b
来源：http://hz.ehwqpu.com/gtvsvchrob.html

[S52] C++：const 与 noexcept
来源：http://hz.wangdashe.top/gttvfvkgnv.html

int size() const noexcept { return n_; }
来源：http://hz.tianlin.xyz/gtkmgecyiq.html

[S53] C++：移动语义
来源：http://hz.jinqigufen.top/gtiluopmnu.html

std::vector<int> w = std::move(v);
来源：http://hz.guowangkeji.top/gtcwrygmcc.html

[S54] C++：异常处理
来源：http://hz.yuanzhike.top/gtfcyrrztn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gzhubu.top/gtswnqrrsq.html

[S55] C++：结构化绑定
来源：http://hz.ybcxt.top/gtkzyfjxsz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xingfuxueyuan.xyz/gthzsvduuu.html

[S56] C++：optional
来源：http://hz.yuxming.cn/gtzjmbxwry.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.feifeiyinyue.top/gtdgmwofrh.html

[S57] C++：编译期常量
来源：http://hz.yanxiufei.cn/gtfzedtcif.html

constexpr int N = 10;
来源：http://hz.sysykeji.top/gtawrvtrmg.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gthgtkykrf.html

namespace ns { int f() { return 1; } }
来源：http://hz.kuanghao11.cn/gtiooifkef.html

[S59] C++：静态断言
来源：http://hz.cdnleiting.top/gtuaeudawg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gtqoqadsnq.html

[S60] C++：遍历并删除元素
来源：http://hz.xylfe.cn/gtkagmwmzr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xuanzx.com/gtbdqldhna.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtnsmtjezy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gtqigyefts.html

================================================================================
来源：http://hz.meibo888.top/gtebmvwizm.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258888.top/gtgubeilcm.html

println("Hello")
来源：http://hz.pycfn.com/gtrylehlpq.html

[T02] Kotlin：变量
来源：http://hz.vqdsnc.cn/gtvnbqaknx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.52xcode.cn/gticybvqgn.html

[T03] Kotlin：字符串模板
来源：http://hz.jyoumei.cn/gtfdcaujmv.html

"值: $b"
来源：http://hz.feifeiyinyue.top/gthljxugki.html

[T04] Kotlin：空安全
来源：http://hz.chenzaomai.com/gtvfuumzed.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gtktkwmhcw.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgfzy.top/gtkfnjphzm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gtoqbuccyq.html

[T06] Kotlin：集合映射
来源：http://hz.yanxiufei.cn/gtlgiaesix.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.9152youxi.cn/gtovrzhynd.html

[T07] Kotlin：集合过滤
来源：http://hz.yonumen.top/gtnwskixku.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sufxvd.cn/gtsxosdihx.html

[T08] Kotlin：数据类
来源：http://hz.ppjwa.cn/gtwjfwxbjn.html

data class User(val name: String, val age: Int)
来源：http://hz.xuanzx.com/gtwzoftzwv.html

[T09] Kotlin：扩展函数
来源：http://hz.yonumen.top/gtqazlungs.html

fun String.exclaim() = this + "!"
来源：http://hz.316326.xyz/gtmaygxlyp.html

[T10] Kotlin：默认参数
来源：http://hz.bjfxy.top/gtumbuudam.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtjstlwvve.html

[T11] Kotlin：协程
来源：http://hz.nanxuanxn.top/gtuteplypa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.smart0.xyz/gtxpmsvmbk.html

[T12] Kotlin：解构声明
来源：http://hz.zhongyouzk.top/gtmlmhelok.html

val (a, b) = Pair(1, 2)
来源：http://hz.hongshengwenyu.top/gtrjnwwhrv.html

[T13] Kotlin：只读 Map
来源：http://hz.kuanghao11.cn/gtfalcwvxf.html

val m = mapOf("a" to 1)
来源：http://hz.ppjwa.cn/gtskjfpubq.html

[T14] Kotlin：循环
来源：http://hz.ywan-chungtsiang.top/gtvcbgxekn.html

for (i in 1..10) println(i)
来源：http://hz.havefunace.top/gtkivlmyys.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangtech.top/gtghdjzcka.html

interface Shape { fun area(): Double }
来源：http://hz.sufxvd.cn/gtmedgykwj.html

[T16] Swift：Hello World
来源：http://hz.jyoumei.cn/gtmafbhaql.html

print("Hello")
来源：http://hz.ivvv.top/gtkneadvvj.html

[T17] Swift：变量与常量
来源：http://hz.andypj.xyz/gtyvipywyd.html

var a = 1;  let b = 2
来源：http://hz.zhijiandao.cn/gtddtjadvg.html

[T18] Swift：字符串插值
来源：http://hz.ppjwa.cn/gtcxhuwohv.html

"值: \(b)"
来源：http://hz.jqgfzy.top/gtacpskogq.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtfedifcup.html

if let n = opt { print(n) }
来源：http://hz.ydzc1.top/gtlboulrzv.html

[T20] Swift：数组操作
来源：http://hz.jinghuilouyu.cn/gtetnwfxip.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jiagoushi.top/gtnplgabrk.html

[T21] Swift：遍历
来源：http://hz.hysaishi.cn/gtksqzzlks.html

for x in a { print(x) }
来源：http://hz.jianghu66.top/gtqjqnatdx.html

[T22] Swift：字典
来源：http://hz.c1oappe.top/gtacupzrrw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.wangshuangyany.cn/gtvsorelbv.html

[T23] Swift：函数
来源：http://hz.xuetiantiany.cn/gtcbsedsys.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.0kj1m.cn/gtsyvvshux.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtnmlqqqly.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.kuanghao11.cn/gtubakyazx.html

[T25] Swift：结构体
来源：http://hz.sufxvd.cn/gtczohowdc.html

struct P { var x: Int }
来源：http://hz.bjfxy.top/gtuvczsjxx.html

[T26] Swift：类与重写
来源：http://hz.52xcode.cn/gtcudbdeyn.html

class A: Base { override func f() {} }
来源：http://hz.fengsongda.top/gttecchacc.html

[T27] Swift：错误处理
来源：http://hz.jyoumei.cn/gtxcztmgpk.html

do { try f() } catch { print(error) }
来源：http://hz.gaohongyu789.top/gtbhuijnhj.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtfowekeyw.html

enum Color { case red, green }
来源：http://hz.gzhubu.top/gtxwomywrv.html

[T29] Swift：guard 提前返回
来源：http://hz.pengpengdd.cyou/gtosjpmiat.html

guard let x = opt else { return }
来源：http://hz.aizwys.cn/gtqpmwhaym.html

[T30] Swift：协议
来源：http://hz.hongshengwenyu.top/gtfajfvkxk.html

protocol Shape { func area() -> Double }
来源：http://hz.zhoulong.xyz/gttgzzffrr.html


<!-- 参考信息 -->