代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cqqwz.cn/gtxnemokgl.html

[R24] 大小写转换
来源：http://hz.sweek.top/gturgefmou.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhixingplan.top/gtlnlgfwzu.html

[R25] 去后缀 / 去前缀
来源：http://hz.shangyingyoupin.top/gtteddupmp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtretdlhfo.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gthpurazrl.html

now=$(date +%F); echo "$now"
来源：http://hz.ppjwa.cn/gtjkyrbhgd.html

[R27] 算术展开
来源：http://hz.yongpay.top/gtuddgfkbt.html

echo $((1 + 2 * 3))
来源：http://hz.ydzc1.top/gtpxpjlsxh.html

[R28] 浮点运算
来源：http://hz.zycfv.cn/gtwinwoseo.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuetiantiany.cn/gtwuzgwwab.html

[R29] 定义函数
来源：http://hz.jlsjyb.cn/gtoikobkzj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xinyue.icu/gtogtjxrtt.html

[R30] 函数返回状态码
来源：http://hz.fzhhl.top/gttwpqjlav.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtcknwvoyr.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gtfsxjsnat.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangkeji.top/gtiumftubh.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtbyflxpfe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.vqdsnc.cn/gtgtwtaaln.html

[R33] 捕获错误并提示行号
来源：http://hz.svipenyu.cn/gtikfdldnn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgufenzy.top/gthpaeklwb.html

[R34] 退出时清理
来源：http://hz.tian-w.cn/gtbkwcaebt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtflaankhi.html

[R35] 后台执行并等待
来源：http://hz.smart0.xyz/gtdtrvftrm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pycfn.com/gtzarqrjxu.html

[R36] 并发执行多个任务
来源：http://hz.hfpthk.cn/gtxgxyadgw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxinkj.top/gtjuyuqjju.html

[R37] 把输出赋给变量
来源：http://hz.hywenlv.cn/gtzuwahmzm.html

files=$(ls -1)
来源：http://hz.sysykeji.top/gtbdkfypnd.html

[R38] 管道串联
来源：http://hz.guannengcc.top/gtorvlgpuo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhijiandao.cn/gtfsspvbqh.html

[R39] 重定向标准输出与错误
来源：http://hz.yanxiufei.cn/gtjgmjlymo.html

cmd > out.log 2>&1
来源：http://hz.pycfn.com/gtkqlaaagd.html

[R40] 追加写日志
来源：http://hz.yvedp.cn/gtwjfjsovk.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtfzcgjmsc.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtxvlmvzhn.html

cmd >/dev/null 2>&1
来源：http://hz.jiagoushi.top/gtqwyhcmas.html

[R42] 输入重定向
来源：http://hz.yj20258.top/gtjfjceedz.html

wc -l < a.txt
来源：http://hz.ydzc1.top/gtchvsedcl.html

[R43] 按名字查找文件
来源：http://hz.yueranfly.top/gtmbwsnttv.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gthzrpyavn.html

[R44] 按修改时间查找
来源：http://hz.iojbl.cn/gtwkzalrsu.html

find . -mtime -7 -type f
来源：http://hz.zycfv.cn/gtffvigdht.html

[R45] 批量删除
来源：http://hz.yj20258888.top/gtabirmqan.html

find . -name "*.tmp" -delete
来源：http://hz.yvedp.cn/gtflzhchwh.html

[R46] 递归替换文件内容
来源：http://hz.aibaodan.cn/gtvrtwkgbz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenlongwang.top/gtogzgacro.html

[R47] sed 单行替换
来源：http://hz.sufxvd.cn/gtnytukgdj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuanzx.com/gtpvkyncob.html

[R48] awk 取指定列
来源：http://hz.cashguo.top/gtapznhayq.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtjjutqcye.html

[R49] awk 带条件
来源：http://hz.52xcode.cn/gtykjxhjvp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtirfnvfym.html

[R50] awk 求和
来源：http://hz.cdnleiting.top/gtxyddwfro.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenjidiqi.icu/gttdkjdnbq.html

[R51] 排序去重取前几
来源：http://hz.jianghu66.top/gtfijmkeqp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guannengcc.top/gtanhmztnx.html

[R52] 统计行数
来源：http://hz.chenzaomai.com/gtgkglbcqx.html

wc -l a.txt
来源：http://hz.jianghu66.top/gtgqeksbva.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258888.top/gtmsxrlmqx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhiwuduotai.top/gtxflpdeuc.html

[R54] 比较两个文件
来源：http://hz.xylfe.cn/gtrrpramgp.html

diff a.txt b.txt
来源：http://hz.xinyue.icu/gtrdfpvcxe.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtskuparly.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtfjuedfrh.html

[R56] 远程拷贝
来源：http://hz.yangfankeji.com/gtetrnvgcw.html

scp file user@host:/path/
来源：http://hz.redwolf501.top/gtmduveuha.html

[R57] 远程执行命令
来源：http://hz.ydjk.org.cn/gtudwislkj.html

ssh user@host 'uptime'
来源：http://hz.bjfxy.top/gtnzwknaau.html

[R58] 下载文件
来源：http://hz.yvedp.cn/gtjxfdchdc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.c1oappe.top/gtapmjudzl.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gteyytpwgm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ehwqpu.com/gtnpjvxpej.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenzaomai.com/gthzekmskt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gthesvvhqf.html

[R61] 磁盘占用
来源：http://hz.sxryk.cn/gtzcysnjhj.html

df -h;  du -sh *
来源：http://hz.zhixingplan.top/gtpafhrykd.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gttyoezlzy.html

du -ah . | sort -rh | head -10
来源：http://hz.cashguo.top/gthewimeqm.html

[R63] 内存与进程
来源：http://hz.aizwys.cn/gtalamswuf.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxuanxn.top/gtarfwklsb.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtmsdswgjl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gtxjpnnrlr.html

[R65] 查看端口占用
来源：http://hz.snrcjt.cn/gthqxoungx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.feifeiyinyue.top/gtxspolcpa.html

[R66] 定时任务
来源：http://hz.ydjk.org.cn/gtacntntyg.html

crontab -e;  crontab -l
来源：http://hz.hammf.cn/gtfonbzhoi.html

[R67] 生成随机十六进制串
来源：http://hz.316326.xyz/gtnzvttncr.html

openssl rand -hex 16
来源：http://hz.shangyingyoupin.top/gtezdbrzjb.html

[R68] 计算文件校验值
来源：http://hz.zhoulong.xyz/gtqwzffmti.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtflmgcfqc.html

[R69] 生成随机密码
来源：http://hz.nanxinkj.top/gtljtiapsh.html

head -c 16 /dev/urandom | base64
来源：http://hz.bjfxy.top/gtuxaoxmur.html

[R70] 时间戳与互转
来源：http://hz.sysykeji.top/gtzgyzkhqq.html

date +%s;  date -d @1700000000
来源：http://hz.jqgufenzy.top/gtsifowskq.html

[R71] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtiasdfkgm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xylfe.cn/gtsujldqqn.html

[R72] 等待端口就绪
来源：http://hz.cucudq.cn/gtpixkloef.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.redwolf501.top/gticzdpmwk.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gtfgjcggpx.html

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtzrhlcdnb.html

[R74] 批量重命名
来源：http://hz.hysaishi.cn/gtlmrkllau.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gtxgmpvorc.html

[R75] 导出环境变量
来源：http://hz.bjfxy.top/gtpjhvaemp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tian-w.cn/gtmhtxvjed.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtjcazwhwq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtmirzonpr.html

[R77] 读取用户输入
来源：http://hz.jyoumei.cn/gtgmflxnvu.html

read -rp "请输入: " ans
来源：http://hz.cdnleiting.top/gtbnwgyxbz.html

[R78] 交互式菜单
来源：http://hz.zycfv.cn/gtllksskwd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhiwuduotai.top/gtpiowhpro.html

[R79] 解析命令行选项
来源：http://hz.ydzc1.top/gtqjytduxt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ivvv.top/gtkigucarz.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxinkj.top/gtuiniarhu.html

time ./run.sh
来源：http://hz.aizwys.cn/gtseixyogi.html

================================================================================
来源：http://hz.ydjk.org.cn/gtheulstge.html

S. C / C++ 专题
来源：http://hz.nanxuanxn.top/gtbmgdxsyo.html

================================================================================
来源：http://hz.yj20258888.top/gtlsxbfqip.html

[S01] C：Hello World
来源：http://hz.ppjwa.cn/gtnkqratjc.html

#include <stdio.h>
来源：http://hz.wangdashe.top/gtkuxlvcke.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuanzhike.top/gtcmuxtvma.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtlrwhmjms.html

int a = 10; printf("%d\n", a);
来源：http://hz.cheryme.top/gtiypwjlux.html

[S03] C：读入整数
来源：http://hz.zhaomingkeji.xyz/gtuwnviwhm.html

int x; scanf("%d", &x);
来源：http://hz.hysaishi.cn/gtnvjxgjrw.html

[S04] C：字符串复制
来源：http://hz.svipenyu.cn/gtcgscxgpc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ywan-chungtsiang.top/gthjkswwhq.html

[S05] C：字符串长度
来源：http://hz.svipenyu.cn/gtxdniruah.html

strlen(s)
来源：http://hz.guannengcc.top/gtxrgwtpyb.html

[S06] C：字符串比较
来源：http://hz.shuidangran.top/gtdxkwutxt.html

strcmp(a, b) == 0
来源：http://hz.tianlin.xyz/gtixxcopyn.html

[S07] C：数组遍历求和
来源：http://hz.ydzc1.top/gtslfdplaa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cheryme.top/gtpsilfkyu.html

[S08] C：动态内存分配与释放
来源：http://hz.havefunace.top/gtvlpblgjz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.andypj.xyz/gtfexlbash.html

[S09] C：结构体定义与初始化
来源：http://hz.pycfn.com/gtrmzltjch.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangshuangyany.cn/gtpxggpdbv.html

[S10] C：指针与解引用
来源：http://hz.jinghuilouyu.cn/gtfvgsgjys.html

int *p = &a;  *p = 5;
来源：http://hz.daria6918.cn/gtkazmxwsa.html

[S11] C：逐行读文件
来源：http://hz.birdmap.top/gtsezqkkwb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtfasjqaiu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hongshengwenyu.top/gtddynppue.html

fclose(f);
来源：http://hz.zdqjudy.top/gteiidxzzv.html

[S12] C：写文件
来源：http://hz.daria6918.cn/gtkrawnbds.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ehwqpu.com/gteckrdeoj.html

[S13] C：宏定义
来源：http://hz.chenjidiqi.icu/gthxyrunjw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jlsjyb.cn/gtmxyvhhpd.html

[S14] C：枚举
来源：http://hz.chenlongwang.top/gtpzunpdax.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.bjfxy.top/gtujdzmgpm.html

[S15] C：类型转换
来源：http://hz.shangyingyoupin.top/gtiuqolcoa.html

(double) a / b
来源：http://hz.wangshuangyany.cn/gtaijoeqjf.html

[S16] C：位操作置位
来源：http://hz.mhx1999.top/gtkbbdpile.html

x |= (1 << 3);
来源：http://hz.sufxvd.cn/gtczbgdosk.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtlffvocnt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhongyouzk.top/gtfbnxaspx.html

[S18] C：命令行参数
来源：http://hz.jqgufenzy.top/gtftzjisxl.html

int main(int argc, char **argv)
来源：http://hz.guowangkeji.top/gtxjhmwkqz.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gteuwegvos.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtianajzsg.html

[S20] C：二分查找
来源：http://hz.meibo888.top/gtelorsytc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gzhubu.top/gtdpcmilgi.html

[S21] C：字符类别判断
来源：http://hz.nwbrower.top/gtahiwrvue.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sxryk.cn/gtemocdwvu.html

[S22] C：字符串转数字
来源：http://hz.daxiang520.top/gtbayxzatr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zycfv.cn/gtrnbecvgx.html

[S23] C：随机数
来源：http://hz.daria6918.cn/gtxwpmgdph.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ywan-chungtsiang.top/gtqmtatuvw.html

[S24] C：获取本地时间
来源：http://hz.ppjwa.cn/gtaipagzqp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sweek.top/gteriarmxj.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtwhltdbsw.html

memcpy(dst, src, n);
来源：http://hz.zhongyouzk.top/gtkxdfdsfi.html

[S26] C：内存清零
来源：http://hz.ehwqpu.com/gtrwyzjlrq.html

memset(a, 0, sizeof a);
来源：http://hz.tianlin.xyz/gtuufijkle.html

[S27] C：定义常量
来源：http://hz.sysykeji.top/gtlgpnqwms.html

const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtecciltcg.html

[S28] C：静态变量
来源：http://hz.yj20258.top/gtgeppodcb.html

static int counter = 0;
来源：http://hz.shangyingyoupin.top/gtgrvynoym.html

[S29] C：变参函数
来源：http://hz.jqgfzy.top/gtwksindrk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.birdmap.top/gtnwibduky.html

[S30] C：头文件保护
来源：http://hz.svipenyu.cn/gtcsvufzjy.html

#ifndef X_H
来源：http://hz.mhx1999.top/gtopuygmmz.html

#define X_H
来源：http://hz.zycfv.cn/gtcuvhwnax.html

#endif
来源：http://hz.aibaodan.cn/gtrknijced.html

[S31] C++：Hello World
来源：http://hz.zycfv.cn/gtipemsllp.html

#include <iostream>
来源：http://hz.kuanghao11.cn/gtlplkatbr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtrmkrszzh.html

[S32] C++：字符串
来源：http://hz.wangshuangyany.cn/gtdlunqltj.html

std::string s = "hi";  s += "!";
来源：http://hz.haohaochexian.top/gtnuvnvfol.html

[S33] C++：vector 增删
来源：http://hz.ybcxt.top/gtmudimosc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yvedp.cn/gtmsxuidsv.html

[S34] C++：遍历 vector
来源：http://hz.cdnleiting.top/gtnsibgvzq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dashuyun.cn/gtvridedgu.html

[S35] C++：map
来源：http://hz.kuanghao11.cn/gtndvoozlb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtlzzdfqdk.html

[S36] C++：unordered_map
来源：http://hz.xziqi.cn/gtynpjppwz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtozyjihvg.html

[S37] C++：set
来源：http://hz.ivvv.top/gtegqhyrea.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xylfe.cn/gttgrlwvcm.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtaikzpffn.html

std::sort(v.begin(), v.end());
来源：http://hz.iojbl.cn/gtuzziwvvv.html

[S39] C++：自定义比较器排序
来源：http://hz.jinyuanbaomall.cn/gtajequsgm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guowangkeji.top/gtecqsmrzd.html

[S40] C++：查找元素
来源：http://hz.xylfe.cn/gtgemrfmfi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtnhrsrokp.html

[S41] C++：类与构造函数
来源：http://hz.bjfxy.top/gtefkfsezj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.birdmap.top/gtibyhknqb.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtxzsrsdhy.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangshuangyany.cn/gtmhypdggg.html

[S43] C++：智能指针
来源：http://hz.pengpengdd.cyou/gteglgkdrm.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinghuilouyu.cn/gtnvxsheeu.html

[S44] C++：引用传参
来源：http://hz.316326.xyz/gttmrktqkq.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gtzacxnxyd.html

[S45] C++：lambda
来源：http://hz.9152youxi.cn/gtaoiqvhsq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.9152youxi.cn/gtjnetwyzn.html

[S46] C++：函数模板
来源：http://hz.zhixingplan.top/gthhbrncdy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhijiandao.cn/gtxgxuefha.html

[S47] C++：结构化绑定遍历
来源：http://hz.meibo888.top/gtudclzyjd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuetiantiany.cn/gtqjhdynqt.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtwffpsbds.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhoulong.xyz/gtoaqikjsh.html

while (std::getline(in, line)) { }
来源：http://hz.shuidangran.top/gtngrfivtx.html

[S49] C++：写文件
来源：http://hz.yvedp.cn/gtmretfugu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigfzy.top/gtfsrwzmjs.html

[S50] C++：格式化数字
来源：http://hz.gotoacloud.top/gtvdkkxnzl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tianlin.xyz/gtpvphubvu.html

[S51] C++：显式类型转换
来源：http://hz.cdnleiting.top/gtgxcztmok.html

static_cast<double>(a) / b
来源：http://hz.wangdashe.top/gtbofhopzy.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgfzy.top/gtteqwzukr.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gtimzbzhds.html

[S53] C++：移动语义
来源：http://hz.ywan-chungtsiang.top/gtewkxfowh.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxuanxn.top/gtbqlrslie.html

[S54] C++：异常处理
来源：http://hz.jianghu66.top/gtafigsvqd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yvedp.cn/gtmwpfoitc.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtupqmgkug.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gthqmvvoyd.html

[S56] C++：optional
来源：http://hz.jiagoushi.top/gtpelhxvat.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yvedp.cn/gtaownmupx.html

[S57] C++：编译期常量
来源：http://hz.daria6918.cn/gtzhknythi.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gtlcvqsric.html

[S58] C++：命名空间
来源：http://hz.zhongyouzk.top/gtxuvxlmbd.html

namespace ns { int f() { return 1; } }
来源：http://hz.jlsjyb.cn/gtqylwcfzl.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtzqbuwizv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aizwys.cn/gtlsngfdtc.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigufen.top/gtadxdemhf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xylfe.cn/gtnajvzbpf.html

================================================================================
来源：http://hz.shzxlz.cn/gttwuclxwt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtauuatbdj.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtcsdtdpmg.html

[T01] Kotlin：Hello World
来源：http://hz.bjfxy.top/gtrzruwisn.html

println("Hello")
来源：http://hz.pycfn.com/gtxuncjlaj.html

[T02] Kotlin：变量
来源：http://hz.yangfankeji.com/gttktkmutb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.guowangkeji.top/gtvvmrfinl.html

[T03] Kotlin：字符串模板
来源：http://hz.kuanghao11.cn/gtyosiqxgy.html

"值: $b"
来源：http://hz.iojbl.cn/gtefgynoau.html

[T04] Kotlin：空安全
来源：http://hz.jinghuilouyu.cn/gthvcfcwcg.html

val n: String? = null;  n?.length
来源：http://hz.yuxming.cn/gtdzlqmdkn.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigufen.top/gtuhiyixdw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgfzy.top/gtuatojctn.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gtjraemnim.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nwbrower.top/gtyfsbfxlh.html

[T07] Kotlin：集合过滤
来源：http://hz.zhoulong.xyz/gtcnrxfiim.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258888.top/gtwokyqsoz.html

[T08] Kotlin：数据类
来源：http://hz.hammf.cn/gtuvuolqrl.html

data class User(val name: String, val age: Int)
来源：http://hz.gzhubu.top/gtgwnhfetn.html

[T09] Kotlin：扩展函数
来源：http://hz.hammf.cn/gtvvlhdvqp.html

fun String.exclaim() = this + "!"
来源：http://hz.fzhhl.top/gtllhwodqi.html

[T10] Kotlin：默认参数
来源：http://hz.yangfankeji.com/gthpcpoykw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yangfankeji.com/gtadkwaawn.html

[T11] Kotlin：协程
来源：http://hz.mhx1999.top/gtgjidkdrd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pycfn.com/gtmqkchqgy.html

[T12] Kotlin：解构声明
来源：http://hz.yongpay.top/gtpfakjaiq.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gtjzyzdwmc.html

[T13] Kotlin：只读 Map
来源：http://hz.ydzc1.top/gtehiukbeu.html

val m = mapOf("a" to 1)
来源：http://hz.pengpengdd.cyou/gtaytghqib.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtksuiwopm.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtupjhiwuo.html

[T15] Kotlin：接口
来源：http://hz.snrcjt.cn/gtduopuudn.html

interface Shape { fun area(): Double }
来源：http://hz.shzxlz.cn/gtdsedrwyb.html

[T16] Swift：Hello World
来源：http://hz.9152youxi.cn/gtgknfccyq.html

print("Hello")
来源：http://hz.tianlin.xyz/gtwrdzaidv.html

[T17] Swift：变量与常量
来源：http://hz.haohaochexian.top/gtuegxrjoj.html

var a = 1;  let b = 2
来源：http://hz.redwolf501.top/gtpgzxjyss.html

[T18] Swift：字符串插值
来源：http://hz.ydzc1.top/gtaakvjesj.html

"值: \(b)"
来源：http://hz.ybcxt.top/gtljbedmll.html

[T19] Swift：可选绑定
来源：http://hz.hongshengwenyu.top/gtgegfaaju.html

if let n = opt { print(n) }
来源：http://hz.haohaochexian.top/gtytfsstqn.html

[T20] Swift：数组操作
来源：http://hz.jqgfzy.top/gtybwhvcqw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtughlbuvl.html

[T21] Swift：遍历
来源：http://hz.xylfe.cn/gtkiyfenrr.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtgzmrrkyy.html

[T22] Swift：字典
来源：http://hz.kuanghao11.cn/gtxymnfner.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yongpay.top/gtuiolngji.html

[T23] Swift：函数
来源：http://hz.ppjwa.cn/gtgzgcnkru.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.quarkkingdee.top/gteufxdjnq.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtvbpevlqt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.c1oappe.top/gttsdzaomv.html

[T25] Swift：结构体
来源：http://hz.zdqjudy.top/gtxfdxlspe.html

struct P { var x: Int }
来源：http://hz.xziqi.cn/gtzojfnplj.html

[T26] Swift：类与重写
来源：http://hz.chenlongwang.top/gthkjdkcal.html

class A: Base { override func f() {} }
来源：http://hz.yueranfly.top/gtlhmcgruh.html


<!-- 参考信息 -->