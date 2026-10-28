代发 wailian999

echo $((1 + 2 * 3))
来源：http://hz.hongshengwenyu.top/gtujfebtri.html

[R28] 浮点运算
来源：http://hz.jianghu66.top/gtxbblikcm.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhiwuduotai.top/gtziotsdtz.html

[R29] 定义函数
来源：http://hz.sweek.top/gthmvhtgkl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.pycfn.com/gtcxrxroun.html

[R30] 函数返回状态码
来源：http://hz.nanxinkj.top/gtupjtumvy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yvedp.cn/gtehgisuzm.html

[R31] 局部变量
来源：http://hz.tian-w.cn/gtfpeoebvm.html

f() { local x=1; echo "$x"; }
来源：http://hz.hywenlv.cn/gtkkapvjoa.html

[R32] 参数个数校验
来源：http://hz.sysykeji.top/gtngkvchck.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhijiandao.cn/gtdowxjmtp.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtfizluisa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jianghu66.top/gtcuqmxtkb.html

[R34] 退出时清理
来源：http://hz.chenlongwang.top/gteqewsobl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtnwyypapm.html

[R35] 后台执行并等待
来源：http://hz.cqqwz.cn/gtodwiehmr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yueranfly.top/gtrggwyipg.html

[R36] 并发执行多个任务
来源：http://hz.jyoumei.cn/gtvjzgebdz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ywan-chungtsiang.top/gtxaowhlxi.html

[R37] 把输出赋给变量
来源：http://hz.svipenyu.cn/gthbkuffls.html

files=$(ls -1)
来源：http://hz.shzxlz.cn/gtbgwhukfb.html

[R38] 管道串联
来源：http://hz.jinyuanbaomall.cn/gtdpkhmbbg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtxkatsutb.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gtbliozgxq.html

cmd > out.log 2>&1
来源：http://hz.chenzaomai.com/gtisgmamjv.html

[R40] 追加写日志
来源：http://hz.xingfuxueyuan.xyz/gttmcnfbyq.html

echo "log" >> out.log
来源：http://hz.hnqzz.top/gtsseyilqr.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtwijyfrjp.html

cmd >/dev/null 2>&1
来源：http://hz.zhongyouzk.top/gtddqpsimy.html

[R42] 输入重定向
来源：http://hz.haohaochexian.top/gtbvlirnnb.html

wc -l < a.txt
来源：http://hz.jinqigufen.top/gtemxyjpvr.html

[R43] 按名字查找文件
来源：http://hz.hfpthk.cn/gthzbxzfxh.html

find . -name "*.log" -type f
来源：http://hz.yuanzhike.top/gtgjdmukkl.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gtgzqpglzg.html

find . -mtime -7 -type f
来源：http://hz.chenjidiqi.icu/gtvlxtrbaj.html

[R45] 批量删除
来源：http://hz.cheryme.top/gtjamsxyeb.html

find . -name "*.tmp" -delete
来源：http://hz.jqgufenzy.top/gtfsixffts.html

[R46] 递归替换文件内容
来源：http://hz.daxiang520.top/gtmwiloopu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.svipenyu.cn/gtsckucojo.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gtqjkqlbda.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gtcrdzcrih.html

[R48] awk 取指定列
来源：http://hz.zhengqikj.top/gtfnddydak.html

awk '{print $1, $3}' a.txt
来源：http://hz.gaohongyu789.top/gtvuvgbpgi.html

[R49] awk 带条件
来源：http://hz.cqqwz.cn/gtcqkxvwui.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258888.top/gtonfqjfga.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtulrxtykg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj202588.top/gtfvihcpck.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtufkcrxbs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tanke756.top/gtjnpaydee.html

[R52] 统计行数
来源：http://hz.vqdsnc.cn/gtsbyishvc.html

wc -l a.txt
来源：http://hz.dianchejie.cn/gtmjqcozgf.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtytqlhmqv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aibaodan.cn/gtseaplfxv.html

[R54] 比较两个文件
来源：http://hz.sxryk.cn/gtesgptksm.html

diff a.txt b.txt
来源：http://hz.jinqigufen.top/gttewpjhse.html

[R55] 压缩与解压
来源：http://hz.feifeiyinyue.top/gtmuivpqne.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtydpyopju.html

[R56] 远程拷贝
来源：http://hz.zycfv.cn/gtshiwepta.html

scp file user@host:/path/
来源：http://hz.cdnleiting.top/gtxlwzzjmr.html

[R57] 远程执行命令
来源：http://hz.jianghu66.top/gtbxollfav.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtuvudulod.html

[R58] 下载文件
来源：http://hz.ydzc1.top/gtfdxyjtvc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hywenlv.cn/gtgepqnuoj.html

[R59] 发 POST JSON
来源：http://hz.cdnleiting.top/gtrqttnoqj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jiagoushi.top/gtbwheqtfn.html

[R60] 只看 HTTP 状态码
来源：http://hz.ppjwa.cn/gtlkohzrak.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sufxvd.cn/gtgqlqqdnu.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtpbhkhczk.html

df -h;  du -sh *
来源：http://hz.svipenyu.cn/gtuvkjhobj.html

[R62] 找最占空间的文件
来源：http://hz.cashguo.top/gtnknsbxze.html

du -ah . | sort -rh | head -10
来源：http://hz.yanxiufei.cn/gtrweaqadk.html

[R63] 内存与进程
来源：http://hz.fzhhl.top/gtovybewnr.html

free -h;  ps aux | grep nginx
来源：http://hz.xziqi.cn/gtektnfbql.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtneajnkfs.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ivvv.top/gtigpsjpfh.html

[R65] 查看端口占用
来源：http://hz.sweek.top/gtsfyawois.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daxiang520.top/gtpcrsjvhh.html

[R66] 定时任务
来源：http://hz.yj202588.top/gtbjrkykyb.html

crontab -e;  crontab -l
来源：http://hz.tian-w.cn/gtmnsjqyok.html

[R67] 生成随机十六进制串
来源：http://hz.smart0.xyz/gtnbwxsukp.html

openssl rand -hex 16
来源：http://hz.52xcode.cn/gtmjtkfuwd.html

[R68] 计算文件校验值
来源：http://hz.hnxiangtu.top/gttahpsbxm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuetiantiany.cn/gtmlbybgnw.html

[R69] 生成随机密码
来源：http://hz.zhijiandao.cn/gtkspdrtgs.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtihowhntq.html

[R70] 时间戳与互转
来源：http://hz.yj20258888.top/gtghnbhgid.html

date +%s;  date -d @1700000000
来源：http://hz.zhengqikj.top/gtiseydrxc.html

[R71] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtjtsahcmm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtrinqdszn.html

[R72] 等待端口就绪
来源：http://hz.jqgufenzy.top/gtklliysak.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hammf.cn/gtjdohtwjs.html

[R73] 分割大日志
来源：http://hz.gzhubu.top/gtaqryrrlj.html

split -l 1000 big.log part_
来源：http://hz.yj202588.top/gtgqotnfac.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtnfuyiwuv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shangyingyoupin.top/gtbxjusrfx.html

[R75] 导出环境变量
来源：http://hz.zhijiandao.cn/gtpfkikqmt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.kuanghao11.cn/gtqxtiemuj.html

[R76] 使用临时文件
来源：http://hz.yanxiufei.cn/gtqdnchtgu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtztnnqdgm.html

[R77] 读取用户输入
来源：http://hz.zhaomingkeji.xyz/gtpvtzxqxd.html

read -rp "请输入: " ans
来源：http://hz.316326.xyz/gtyjlcvrvq.html

[R78] 交互式菜单
来源：http://hz.vqdsnc.cn/gttrjjdusg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydzc1.top/gtjlubrqml.html

[R79] 解析命令行选项
来源：http://hz.jianghu66.top/gtmaptiaws.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtdbtljmcu.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtlqdskiua.html

time ./run.sh
来源：http://hz.yongpay.top/gtqkghigfy.html

================================================================================
来源：http://hz.aizwys.cn/gtihbuwjeh.html

S. C / C++ 专题
来源：http://hz.hongshengwenyu.top/gtdzmhgeli.html

================================================================================
来源：http://hz.guannengcc.top/gtnrvwcptf.html

[S01] C：Hello World
来源：http://hz.mhx1999.top/gtxclywxih.html

#include <stdio.h>
来源：http://hz.xuetiantiany.cn/gtbgufbfoq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ybcxt.top/gtmxiakbkt.html

[S02] C：变量与格式化输出
来源：http://hz.iojbl.cn/gtfhfzskxi.html

int a = 10; printf("%d\n", a);
来源：http://hz.pycfn.com/gtwwfimhaf.html

[S03] C：读入整数
来源：http://hz.cheryme.top/gthnbcwjch.html

int x; scanf("%d", &x);
来源：http://hz.hfpthk.cn/gtuyfeaoci.html

[S04] C：字符串复制
来源：http://hz.cucudq.cn/gtjxhfhxcr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guowangkeji.top/gtsqxxaupr.html

[S05] C：字符串长度
来源：http://hz.nanxuanxn.top/gtheflkesl.html

strlen(s)
来源：http://hz.iojbl.cn/gtqyriuhyk.html

[S06] C：字符串比较
来源：http://hz.sweek.top/gtsraslylp.html

strcmp(a, b) == 0
来源：http://hz.chenjidiqi.icu/gtpsmxpnxo.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtizaujotg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigfzy.top/gtpgimdemr.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gtfzlwogcw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.haohaochexian.top/gtyezuorct.html

[S09] C：结构体定义与初始化
来源：http://hz.zhoulong.xyz/gtaphiqnld.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sweek.top/gtmevmervo.html

[S10] C：指针与解引用
来源：http://hz.yuxming.cn/gttrfiddxd.html

int *p = &a;  *p = 5;
来源：http://hz.hysaishi.cn/gtsfmdywxj.html

[S11] C：逐行读文件
来源：http://hz.havefunace.top/gtwcoiqysn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtmtwdhuio.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.guowangkeji.top/gtuhytjilm.html

fclose(f);
来源：http://hz.aibaodan.cn/gtjhmsvpni.html

[S12] C：写文件
来源：http://hz.zycfv.cn/gtmtvoumzm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gtixeyrcuv.html

[S13] C：宏定义
来源：http://hz.gogol.net.cn/gtixyxhwqa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgufenzy.top/gtmrceralp.html

[S14] C：枚举
来源：http://hz.cdnleiting.top/gtekbmmwai.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cashguo.top/gtzdvtflvk.html

[S15] C：类型转换
来源：http://hz.hywenlv.cn/gtnridgghm.html

(double) a / b
来源：http://hz.zhengqikj.top/gtnwnvjthn.html

[S16] C：位操作置位
来源：http://hz.jiagoushi.top/gtflmvpsbl.html

x |= (1 << 3);
来源：http://hz.9152youxi.cn/gtqwndbldx.html

[S17] C：安全拼接字符串
来源：http://hz.hfpthk.cn/gtaukioeix.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuanzx.com/gtvcqzjnzg.html

[S18] C：命令行参数
来源：http://hz.shzxlz.cn/gtjiybhtzj.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gtgdpyrnkt.html

[S19] C：快速排序
来源：http://hz.gotoacloud.top/gtatiswwpq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.wangshuangyany.cn/gtudaibwin.html

[S20] C：二分查找
来源：http://hz.sweek.top/gtuzyqbxfy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtbmdmiaxf.html

[S21] C：字符类别判断
来源：http://hz.shuidangran.top/gtcyqjwkzf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gtibqarhyd.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtppondnkq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhaomingkeji.xyz/gtiojhxdvw.html

[S23] C：随机数
来源：http://hz.feifeiyinyue.top/gtrjcofyvw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hywenlv.cn/gtnbhpeezk.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gtsqolfzac.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yangfankeji.com/gtbnrisevn.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtzdxmiyzd.html

memcpy(dst, src, n);
来源：http://hz.yonumen.top/gtinzssjhl.html

[S26] C：内存清零
来源：http://hz.zhongyouzk.top/gtcjtptocp.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtwmeqmjpy.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtaivbzpav.html

const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtehzgmija.html

[S28] C：静态变量
来源：http://hz.mhx1999.top/gtkbnnhocg.html

static int counter = 0;
来源：http://hz.redwolf501.top/gtnzakkvwh.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gtktogchdk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnxiangtu.top/gteltqapbx.html

[S30] C：头文件保护
来源：http://hz.dashuyun.cn/gtsnceygva.html

#ifndef X_H
来源：http://hz.zhijiandao.cn/gtxtaptevy.html

#define X_H
来源：http://hz.ydzc1.top/gtvbgesohe.html

#endif
来源：http://hz.hfpthk.cn/gtnhomhrjr.html

[S31] C++：Hello World
来源：http://hz.kuanghao11.cn/gtfefwysdx.html

#include <iostream>
来源：http://hz.jianghu66.top/gtfrlzhruq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sxryk.cn/gtbqljkrcu.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gtygqjsajo.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtzgjlktfu.html

[S33] C++：vector 增删
来源：http://hz.zhongyouzk.top/gtorcsxzqw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yvedp.cn/gtizgztopc.html

[S34] C++：遍历 vector
来源：http://hz.yj202588.top/gtjldqwetq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhixingplan.top/gtczgjebpf.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtkapbgvhb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtnzqthbqf.html

[S36] C++：unordered_map
来源：http://hz.yj202588.top/gtubgnjrpx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigufen.top/gtrlbfwmvx.html

[S37] C++：set
来源：http://hz.zhaomingkeji.xyz/gtkztassyw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.wangdashe.top/gtpdxsycnd.html

[S38] C++：排序
来源：http://hz.gogol.net.cn/gtqfzxcndh.html

std::sort(v.begin(), v.end());
来源：http://hz.ehwqpu.com/gtcrwpmzqw.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtiauqxvzm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guowangkeji.top/gtswwvbvpp.html

[S40] C++：查找元素
来源：http://hz.gzhubu.top/gtphyzsfsv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.0kj1m.cn/gttfgzpkaj.html

[S41] C++：类与构造函数
来源：http://hz.cashguo.top/gtxovpvvsy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zdqjudy.top/gtuqtgkujx.html

[S42] C++：继承与虚函数
来源：http://hz.xziqi.cn/gthtomsmun.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtvvrznvgt.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangkeji.top/gtlforzsbb.html

auto p = std::make_unique<int>(5);
来源：http://hz.pengpengdd.cyou/gtconyfcxp.html

[S44] C++：引用传参
来源：http://hz.sufxvd.cn/gtuikxdyzu.html

void inc(int &x) { ++x; }
来源：http://hz.redwolf501.top/gtaesxocus.html

[S45] C++：lambda
来源：http://hz.gogol.net.cn/gtbvhqgsni.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.quarkkingdee.top/gtixbckujl.html

[S46] C++：函数模板
来源：http://hz.zdqjudy.top/gtvuvcfopm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtktdnbhjg.html

[S47] C++：结构化绑定遍历
来源：http://hz.dashuyun.cn/gtdkctyapo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sysykeji.top/gttjhwngxw.html

[S48] C++：逐行读文件
来源：http://hz.jqgufenzy.top/gtsyaobpbv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtldiiqmlc.html

while (std::getline(in, line)) { }
来源：http://hz.0kj1m.cn/gtnbcnxeyb.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtcmxbtamw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xinyue.icu/gtfceslqir.html

[S50] C++：格式化数字
来源：http://hz.yanxiufei.cn/gtvfwnkenc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.andypj.xyz/gtchebhosi.html

[S51] C++：显式类型转换
来源：http://hz.nanxuanxn.top/gtknssrggv.html

static_cast<double>(a) / b
来源：http://hz.sweek.top/gtkabdksxj.html

[S52] C++：const 与 noexcept
来源：http://hz.feifeiyinyue.top/gthitjdegl.html

int size() const noexcept { return n_; }
来源：http://hz.xziqi.cn/gtnelswvcs.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gttcpkjmsg.html

std::vector<int> w = std::move(v);
来源：http://hz.vqdsnc.cn/gtypsenywt.html

[S54] C++：异常处理
来源：http://hz.chenlongwang.top/gtthopivcx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.aibaodan.cn/gtphcofycj.html

[S55] C++：结构化绑定
来源：http://hz.hysaishi.cn/gtrsqsmevz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtbnfiwydo.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gthkugngeg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.quarkkingdee.top/gtcfotjtwa.html

[S57] C++：编译期常量
来源：http://hz.cashguo.top/gtzsdljmeb.html

constexpr int N = 10;
来源：http://hz.gotoacloud.top/gtodybfmdg.html

[S58] C++：命名空间
来源：http://hz.daxiang520.top/gtjgnrzpue.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtuafopxfw.html

[S59] C++：静态断言
来源：http://hz.jyoumei.cn/gtruzidltw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.52xcode.cn/gtfehrlnhs.html

[S60] C++：遍历并删除元素
来源：http://hz.zhongyouzk.top/gtcjfzkgnq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhongyouzk.top/gtprufweqx.html

================================================================================
来源：http://hz.ydjk.org.cn/gtmadagqls.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gtpiazvkev.html

================================================================================
来源：http://hz.cdnleiting.top/gtvehlsdwa.html

[T01] Kotlin：Hello World
来源：http://hz.jyoumei.cn/gtfhgcsclt.html

println("Hello")
来源：http://hz.fengsongda.top/gtdjdnocro.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangkeji.top/gtbiesifku.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgfzy.top/gtleuepivn.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtjgiyqydn.html

"值: $b"
来源：http://hz.hysaishi.cn/gtwdtbjptd.html

[T04] Kotlin：空安全
来源：http://hz.yj20258888.top/gtavcinnpv.html

val n: String? = null;  n?.length
来源：http://hz.jinqigfzy.top/gtaubojlro.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gtjxcjgkcd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shangyingyoupin.top/gtzewhbmah.html

[T06] Kotlin：集合映射
来源：http://hz.xuetiantiany.cn/gtezfzucej.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.c1oappe.top/gtdqtgrvkf.html

[T07] Kotlin：集合过滤
来源：http://hz.yongpay.top/gtemosrjqu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.mhx1999.top/gtuumtxffc.html

[T08] Kotlin：数据类
来源：http://hz.andypj.xyz/gtrnaaoczu.html

data class User(val name: String, val age: Int)
来源：http://hz.zhongyouzk.top/gtmglznuhh.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigufen.top/gttqgwvnkz.html

fun String.exclaim() = this + "!"
来源：http://hz.daria6918.cn/gtlulumkfq.html

[T10] Kotlin：默认参数
来源：http://hz.sufxvd.cn/gtaxqzaicv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tianlin.xyz/gtujfvfztc.html

[T11] Kotlin：协程
来源：http://hz.nanxuanxn.top/gtlzntsfux.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinyuanbaomall.cn/gtsygfxsnf.html

[T12] Kotlin：解构声明
来源：http://hz.jianghu66.top/gthuohalrf.html

val (a, b) = Pair(1, 2)
来源：http://hz.ppjwa.cn/gtcvnfhhlq.html

[T13] Kotlin：只读 Map
来源：http://hz.chenlongwang.top/gtipuzzjtk.html

val m = mapOf("a" to 1)
来源：http://hz.xinyue.icu/gtfsdrddre.html

[T14] Kotlin：循环
来源：http://hz.dianchejie.cn/gtqbnsmlmw.html

for (i in 1..10) println(i)
来源：http://hz.redwolf501.top/gtcquujlxu.html

[T15] Kotlin：接口
来源：http://hz.jinghuilouyu.cn/gtwjdszami.html

interface Shape { fun area(): Double }
来源：http://hz.ybcxt.top/gtlixmburz.html

[T16] Swift：Hello World
来源：http://hz.zhongyouzk.top/gtrssucmxf.html

print("Hello")
来源：http://hz.ydzc1.top/gtdsdywlzl.html

[T17] Swift：变量与常量
来源：http://hz.bjfxy.top/gtucdxxwaw.html

var a = 1;  let b = 2
来源：http://hz.hammf.cn/gtlydcpjej.html

[T18] Swift：字符串插值
来源：http://hz.bjfxy.top/gtkhkyqrmq.html

"值: \(b)"
来源：http://hz.iojbl.cn/gtbdwzsgrx.html

[T19] Swift：可选绑定
来源：http://hz.tian-w.cn/gtrrrrbith.html

if let n = opt { print(n) }
来源：http://hz.0kj1m.cn/gtiouynbcx.html

[T20] Swift：数组操作
来源：http://hz.zdqjudy.top/gtvijlqcnm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenjidiqi.icu/gtkimvzowp.html

[T21] Swift：遍历
来源：http://hz.yj20258.top/gtgbntmfsi.html

for x in a { print(x) }
来源：http://hz.jyoumei.cn/gtszjbjish.html

[T22] Swift：字典
来源：http://hz.yonumen.top/gttvcgcssc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ppjwa.cn/gtarhxzihz.html

[T23] Swift：函数
来源：http://hz.shanyushiyangtech.top/gtyitjsiln.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jianghu66.top/gtcvfgztrn.html

[T24] Swift：闭包
来源：http://hz.jinqigfzy.top/gtnjzjbqyy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenlongwang.top/gtclavkmox.html

[T25] Swift：结构体
来源：http://hz.redwolf501.top/gtbsoccqpt.html

struct P { var x: Int }
来源：http://hz.aizwys.cn/gtmfhgdtxw.html

[T26] Swift：类与重写
来源：http://hz.andypj.xyz/gtcwxprzts.html

class A: Base { override func f() {} }
来源：http://hz.vqdsnc.cn/gtwajgkjbh.html

[T27] Swift：错误处理
来源：http://hz.mhx1999.top/gtfvopzyvi.html

do { try f() } catch { print(error) }
来源：http://hz.pycfn.com/gtaujetukg.html

[T28] Swift：枚举
来源：http://hz.tian-w.cn/gtdxbktyjl.html

enum Color { case red, green }
来源：http://hz.jqgfzy.top/gtpuuhlevk.html

[T29] Swift：guard 提前返回
来源：http://hz.zycfv.cn/gtobibvncc.html

guard let x = opt else { return }
来源：http://hz.cheryme.top/gtwawexgqr.html

[T30] Swift：协议
来源：http://hz.hongshengwenyu.top/gtzcvmtsdy.html

protocol Shape { func area() -> Double }
来源：http://hz.sxryk.cn/gtuelltgip.html


<!-- 参考信息 -->