代发 wailian999

echo "${#arr[@]}"
来源：http://hz.cashguo.top/gtcimslmiq.html

[R20] 关联数组（字典）
来源：http://hz.quarkkingdee.top/gtrobhbxvc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ppjwa.cn/gtsfnbzquy.html

[R21] 字符串长度
来源：http://hz.sysykeji.top/gtvuibddqt.html

echo "${#s}"
来源：http://hz.havefunace.top/gthfdjdotu.html

[R22] 截取子串
来源：http://hz.zdqjudy.top/gtwnvrylbv.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtvlwlardw.html

[R23] 字符串替换
来源：http://hz.dashuyun.cn/gtbasopcxt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtsqaiyvyd.html

[R24] 大小写转换
来源：http://hz.nanxuanxn.top/gtdpbfupyv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydjk.org.cn/gtyapwbfdu.html

[R25] 去后缀 / 去前缀
来源：http://hz.haohaochexian.top/gtgqhetjgv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nanxuanxn.top/gtkittlthp.html

[R26] 命令替换
来源：http://hz.9152youxi.cn/gtpivzwelp.html

now=$(date +%F); echo "$now"
来源：http://hz.zhiwuduotai.top/gtoundhwzj.html

[R27] 算术展开
来源：http://hz.cucudq.cn/gtwgsalata.html

echo $((1 + 2 * 3))
来源：http://hz.jqgfzy.top/gtcwxcagcx.html

[R28] 浮点运算
来源：http://hz.andypj.xyz/gtntffqvse.html

echo "scale=2; 10/3" | bc
来源：http://hz.nwbrower.top/gtynlfidqs.html

[R29] 定义函数
来源：http://hz.yongpay.top/gteerzxnfv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jiagoushi.top/gtbbbibydm.html

[R30] 函数返回状态码
来源：http://hz.hfpthk.cn/gtuwmclcpb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.c1oappe.top/gtgfpyyenu.html

[R31] 局部变量
来源：http://hz.0kj1m.cn/gtrgmedqay.html

f() { local x=1; echo "$x"; }
来源：http://hz.ppjwa.cn/gtcjolbrss.html

[R32] 参数个数校验
来源：http://hz.tanke756.top/gtuiapugej.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shuidangran.top/gtxyuenvxj.html

[R33] 捕获错误并提示行号
来源：http://hz.zhixingplan.top/gtfhiazina.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gtisrtbuhg.html

[R34] 退出时清理
来源：http://hz.sysykeji.top/gtusgrziwz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtogvlxwyi.html

[R35] 后台执行并等待
来源：http://hz.ydjk.org.cn/gtejwpysmb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtvfnvyjlz.html

[R36] 并发执行多个任务
来源：http://hz.aizwys.cn/gtzbxchwqv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxinkj.top/gtshpbwvus.html

[R37] 把输出赋给变量
来源：http://hz.sweek.top/gtorgfcuzn.html

files=$(ls -1)
来源：http://hz.svipenyu.cn/gtrqnkacjd.html

[R38] 管道串联
来源：http://hz.feifeiyinyue.top/gttwyunnus.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtrosscswr.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gtfxmwjlva.html

cmd > out.log 2>&1
来源：http://hz.nwbrower.top/gtytzwxevc.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtsnkomnho.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gthaccohai.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtwhjfitgs.html

cmd >/dev/null 2>&1
来源：http://hz.kuanghao11.cn/gtyubnohei.html

[R42] 输入重定向
来源：http://hz.gaohongyu789.top/gthvmpualy.html

wc -l < a.txt
来源：http://hz.guannengcc.top/gthccxbznb.html

[R43] 按名字查找文件
来源：http://hz.hnqzz.top/gtqtwspxaj.html

find . -name "*.log" -type f
来源：http://hz.9152youxi.cn/gtbtciwzlq.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gtxndrjmql.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtlpnirrfb.html

[R45] 批量删除
来源：http://hz.zhiwuduotai.top/gtlucaalod.html

find . -name "*.tmp" -delete
来源：http://hz.9152youxi.cn/gtmeyhrcfu.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangkeji.top/gtoluoszuw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenjidiqi.icu/gtgxwpfihj.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gtqbwygwvf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gogol.net.cn/gtlmmzjcau.html

[R48] awk 取指定列
来源：http://hz.gogol.net.cn/gtovjdstyv.html

awk '{print $1, $3}' a.txt
来源：http://hz.vqdsnc.cn/gtvvhiknts.html

[R49] awk 带条件
来源：http://hz.smart0.xyz/gthnvxcgjl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.iojbl.cn/gtywhttxpm.html

[R50] awk 求和
来源：http://hz.yongpay.top/gtyuxxfmmp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jqgufenzy.top/gtdfiptrul.html

[R51] 排序去重取前几
来源：http://hz.ydjk.org.cn/gtyrmhynhc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenjidiqi.icu/gtfotegxmj.html

[R52] 统计行数
来源：http://hz.snrcjt.cn/gtamnxbzfc.html

wc -l a.txt
来源：http://hz.smart0.xyz/gtigoutijn.html

[R53] 查看文件头与实时尾
来源：http://hz.zhongyouzk.top/gtudzwjrqp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shuidangran.top/gtvemgkcmz.html

[R54] 比较两个文件
来源：http://hz.ehwqpu.com/gtflkiijao.html

diff a.txt b.txt
来源：http://hz.wangshuangyany.cn/gttrzzizhq.html

[R55] 压缩与解压
来源：http://hz.daxiang520.top/gtruavvlov.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.feifeiyinyue.top/gtfldpicke.html

[R56] 远程拷贝
来源：http://hz.hysaishi.cn/gttahrbhzj.html

scp file user@host:/path/
来源：http://hz.cashguo.top/gtujauhslv.html

[R57] 远程执行命令
来源：http://hz.smart0.xyz/gtotwqrohm.html

ssh user@host 'uptime'
来源：http://hz.guowangkeji.top/gtntqcudfi.html

[R58] 下载文件
来源：http://hz.pengpengdd.cyou/gtyzsumcch.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.smart0.xyz/gtsdmyfzso.html

[R59] 发 POST JSON
来源：http://hz.52xcode.cn/gtuixjeuup.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhongyouzk.top/gtlasqtunm.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtoonkiurh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.bjfxy.top/gtvmnavryo.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtrkuqelcs.html

df -h;  du -sh *
来源：http://hz.havefunace.top/gtrqtqqpum.html

[R62] 找最占空间的文件
来源：http://hz.nanxuanxn.top/gtkdtruiyv.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtzwjfkhvo.html

[R63] 内存与进程
来源：http://hz.yueranfly.top/gtpixqmqly.html

free -h;  ps aux | grep nginx
来源：http://hz.birdmap.top/gtpgykdatr.html

[R64] 结束进程
来源：http://hz.zhiwuduotai.top/gtzhydzasu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xinyue.icu/gtktekevdh.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangtech.top/gtzgfrgrib.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtjdeljcym.html

[R66] 定时任务
来源：http://hz.gotoacloud.top/gtxbgbbbop.html

crontab -e;  crontab -l
来源：http://hz.mhx1999.top/gtsdsaworq.html

[R67] 生成随机十六进制串
来源：http://hz.xingfuxueyuan.xyz/gtvtgkgjxy.html

openssl rand -hex 16
来源：http://hz.hywenlv.cn/gtmiqpxdyk.html

[R68] 计算文件校验值
来源：http://hz.ivvv.top/gtidyimxid.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aizwys.cn/gtrdsrbbfv.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtsdsltdxr.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtpnpbovgf.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangkeji.top/gtiqcuimub.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtfmvmhuzd.html

[R71] 日期格式化
来源：http://hz.cucudq.cn/gtnsnzlted.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenlongwang.top/gtlamidwku.html

[R72] 等待端口就绪
来源：http://hz.zhaomingkeji.xyz/gtdlyhhnfx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtdpzczpls.html

[R73] 分割大日志
来源：http://hz.smart0.xyz/gtviaezmxq.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtqomzorlc.html

[R74] 批量重命名
来源：http://hz.sxryk.cn/gtlehcoxjw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj202588.top/gtascmmpze.html

[R75] 导出环境变量
来源：http://hz.hfpthk.cn/gtwitutufu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cheryme.top/gtpixoanws.html

[R76] 使用临时文件
来源：http://hz.yj20258888.top/gtwlrvuudf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtkojfjymw.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gtrowgcvzh.html

read -rp "请输入: " ans
来源：http://hz.sysykeji.top/gtawelavcc.html

[R78] 交互式菜单
来源：http://hz.zhengqikj.top/gtuldwbjor.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.andypj.xyz/gtvosnxais.html

[R79] 解析命令行选项
来源：http://hz.cucudq.cn/gtfolgkyfq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.316326.xyz/gtcajrbutk.html

[R80] 查看脚本执行耗时
来源：http://hz.ivvv.top/gtqapbuauv.html

time ./run.sh
来源：http://hz.yj202588.top/gtqxcrncwa.html

================================================================================
来源：http://hz.dianchejie.cn/gtuklofalk.html

S. C / C++ 专题
来源：http://hz.jqgufenzy.top/gtykmsuhfi.html

================================================================================
来源：http://hz.nwbrower.top/gtcpzrhrql.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gtcxpatnnl.html

#include <stdio.h>
来源：http://hz.gogol.net.cn/gtjvlqnuub.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.mhx1999.top/gteeeetfsh.html

[S02] C：变量与格式化输出
来源：http://hz.shuidangran.top/gtwyxidlah.html

int a = 10; printf("%d\n", a);
来源：http://hz.haohaochexian.top/gttqvmuxak.html

[S03] C：读入整数
来源：http://hz.svipenyu.cn/gtrrpswxbd.html

int x; scanf("%d", &x);
来源：http://hz.chenzaomai.com/gtyqbbcmbd.html

[S04] C：字符串复制
来源：http://hz.yueranfly.top/gtcficmzwv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenlongwang.top/gtppelstyy.html

[S05] C：字符串长度
来源：http://hz.hywenlv.cn/gtejtvqgse.html

strlen(s)
来源：http://hz.nwbrower.top/gtyixpnasw.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtabqwpfwz.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gtbxawnwau.html

[S07] C：数组遍历求和
来源：http://hz.zhongyouzk.top/gtnznmsqrm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnxiangtu.top/gtzfhxrwst.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gtprpqualx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgfzy.top/gtjygppdyc.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtqltndqdf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.meibo888.top/gtsuvierub.html

[S10] C：指针与解引用
来源：http://hz.hongshengwenyu.top/gtmsvwinzm.html

int *p = &a;  *p = 5;
来源：http://hz.smart0.xyz/gthslptquy.html

[S11] C：逐行读文件
来源：http://hz.pycfn.com/gthmpykqex.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gtoamzfsya.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtopmvuele.html

fclose(f);
来源：http://hz.hongshengwenyu.top/gtbcqpgwls.html

[S12] C：写文件
来源：http://hz.cucudq.cn/gtgxocxmcp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yongpay.top/gthzjkjkiu.html

[S13] C：宏定义
来源：http://hz.yangfankeji.com/gtbmdqfsal.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtxsqtcwui.html

[S14] C：枚举
来源：http://hz.birdmap.top/gtmnpkgvag.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shangyingyoupin.top/gtiykqxdab.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtepfcrejh.html

(double) a / b
来源：http://hz.bjfxy.top/gtkisjunix.html

[S16] C：位操作置位
来源：http://hz.jyoumei.cn/gteewfarse.html

x |= (1 << 3);
来源：http://hz.zhongyouzk.top/gtojgruwyl.html

[S17] C：安全拼接字符串
来源：http://hz.aizwys.cn/gtelwwyaby.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj202588.top/gtstfzljst.html

[S18] C：命令行参数
来源：http://hz.zhoulong.xyz/gtzeujbzjt.html

int main(int argc, char **argv)
来源：http://hz.yuanzhike.top/gtjxyiekyx.html

[S19] C：快速排序
来源：http://hz.cqqwz.cn/gtwdhcdehj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtkdbktvsx.html

[S20] C：二分查找
来源：http://hz.52xcode.cn/gtqbhlsjgw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtxfjzzzqz.html

[S21] C：字符类别判断
来源：http://hz.cucudq.cn/gtblxzbzkx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinghuilouyu.cn/gtiwzmmzjx.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtsxsyiuij.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtgzoippsp.html

[S23] C：随机数
来源：http://hz.yanxiufei.cn/gtrtfewhbq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgufenzy.top/gttcbkmhvz.html

[S24] C：获取本地时间
来源：http://hz.nanxinkj.top/gtoonicnvl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtdrajuonf.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gtxcgnwvcu.html

memcpy(dst, src, n);
来源：http://hz.pengpengdd.cyou/gtifzxeeex.html

[S26] C：内存清零
来源：http://hz.birdmap.top/gtlfyflqam.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtwpklozhs.html

[S27] C：定义常量
来源：http://hz.nwbrower.top/gtmsgjrobb.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtuhoxsnwx.html

[S28] C：静态变量
来源：http://hz.zhengqikj.top/gtfvuhqljn.html

static int counter = 0;
来源：http://hz.zhongyouzk.top/gtlvwytbrb.html

[S29] C：变参函数
来源：http://hz.zhiwuduotai.top/gtppzasdlf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangdashe.top/gtwslgwgiy.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtcsdjoaty.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtjizmmmoq.html

#define X_H
来源：http://hz.yangfankeji.com/gttiiomuup.html

#endif
来源：http://hz.jinqigufen.top/gtwkxuidtv.html

[S31] C++：Hello World
来源：http://hz.nanxuanxn.top/gtwkywtvxw.html

#include <iostream>
来源：http://hz.mhx1999.top/gtiiozcepj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.redwolf501.top/gtfvcqjvlj.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gtzicrxrck.html

std::string s = "hi";  s += "!";
来源：http://hz.xziqi.cn/gtgikwbytt.html

[S33] C++：vector 增删
来源：http://hz.nanxuanxn.top/gtltvhrxyj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dashuyun.cn/gtbnelwbil.html

[S34] C++：遍历 vector
来源：http://hz.gaohongyu789.top/gteuiontfd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jqgfzy.top/gtmhydpwir.html

[S35] C++：map
来源：http://hz.zhongyouzk.top/gtpqgmeegt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtchyrzexj.html

[S36] C++：unordered_map
来源：http://hz.tianlin.xyz/gtllvpkwrr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtobfweibg.html

[S37] C++：set
来源：http://hz.sweek.top/gtqsurrmpv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shangyingyoupin.top/gtcfnerete.html

[S38] C++：排序
来源：http://hz.hywenlv.cn/gtfaxgnifw.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtxmrxrvei.html

[S39] C++：自定义比较器排序
来源：http://hz.cucudq.cn/gtjoopqcwc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.andypj.xyz/gtahhsptaa.html

[S40] C++：查找元素
来源：http://hz.smart0.xyz/gtqnmvjscl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtjpvyrfyk.html

[S41] C++：类与构造函数
来源：http://hz.zhengqikj.top/gtbtkvodbj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tianlin.xyz/gtgxnlnxbb.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258.top/gtapasjfdo.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinyuanbaomall.cn/gtcsgsurxt.html

[S43] C++：智能指针
来源：http://hz.meibo888.top/gtmhaskinr.html

auto p = std::make_unique<int>(5);
来源：http://hz.daria6918.cn/gtbqfuaqlu.html

[S44] C++：引用传参
来源：http://hz.fzhhl.top/gtilynyxtp.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtzlqpluwa.html

[S45] C++：lambda
来源：http://hz.ppjwa.cn/gtttmkdhvf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gtsioftcnx.html

[S46] C++：函数模板
来源：http://hz.jqgfzy.top/gttuxyvllx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtdgatpsac.html

[S47] C++：结构化绑定遍历
来源：http://hz.birdmap.top/gtugtgeqao.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hammf.cn/gtyaymdoet.html

[S48] C++：逐行读文件
来源：http://hz.hongshengwenyu.top/gtczzlatwx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jiagoushi.top/gtrbznnwcu.html

while (std::getline(in, line)) { }
来源：http://hz.mhx1999.top/gtemehnryk.html

[S49] C++：写文件
来源：http://hz.nanxuanxn.top/gtjvhqpyho.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtbqnvlxos.html

[S50] C++：格式化数字
来源：http://hz.daxiang520.top/gtypijbegt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ivvv.top/gtunyohore.html

[S51] C++：显式类型转换
来源：http://hz.shuidangran.top/gtvugirwqt.html

static_cast<double>(a) / b
来源：http://hz.cqqwz.cn/gtunnlonrj.html

[S52] C++：const 与 noexcept
来源：http://hz.dashuyun.cn/gtaputvino.html

int size() const noexcept { return n_; }
来源：http://hz.yj202588.top/gtcudxukie.html

[S53] C++：移动语义
来源：http://hz.gaohongyu789.top/gtnsscaift.html

std::vector<int> w = std::move(v);
来源：http://hz.ivvv.top/gtdpfvraby.html

[S54] C++：异常处理
来源：http://hz.jinqigfzy.top/gtogojnjvm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigufen.top/gtzhfokwld.html

[S55] C++：结构化绑定
来源：http://hz.smart0.xyz/gtwttbyyqb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenlongwang.top/gtiwnbdzht.html

[S56] C++：optional
来源：http://hz.jinghuilouyu.cn/gtpatcsaiv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.andypj.xyz/gtdlurruhm.html

[S57] C++：编译期常量
来源：http://hz.havefunace.top/gtegoizvly.html

constexpr int N = 10;
来源：http://hz.sweek.top/gtpdccdipc.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtmbhnzhuk.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuetiantiany.cn/gtiaxqldfb.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtzfpyvrev.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinyuanbaomall.cn/gtqzsmlzqa.html

[S60] C++：遍历并删除元素
来源：http://hz.gzhubu.top/gtyjksteof.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.svipenyu.cn/gtmlnfgofn.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtnzsquqbu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.mhx1999.top/gtixehmsdy.html

================================================================================
来源：http://hz.yj20258.top/gtlrwcqxfs.html

[T01] Kotlin：Hello World
来源：http://hz.zycfv.cn/gtrvnlxsgb.html

println("Hello")
来源：http://hz.cqqwz.cn/gteksfbuzj.html

[T02] Kotlin：变量
来源：http://hz.kuanghao11.cn/gtdmvwlfba.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zdqjudy.top/gtcdqjtetu.html

[T03] Kotlin：字符串模板
来源：http://hz.zhongyouzk.top/gtpfpcrjok.html

"值: $b"
来源：http://hz.yangfankeji.com/gtapsrhiiw.html

[T04] Kotlin：空安全
来源：http://hz.sysykeji.top/gtwmfixcei.html

val n: String? = null;  n?.length
来源：http://hz.xziqi.cn/gthgzpuxdw.html

[T05] Kotlin：when 表达式
来源：http://hz.jlsjyb.cn/gtooqidjbr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gtplnooqol.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gtdrcpetct.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.svipenyu.cn/gtgmagwsmq.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtxvttjlem.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cucudq.cn/gtevnuvgzz.html

[T08] Kotlin：数据类
来源：http://hz.hfpthk.cn/gtwifkrndb.html

data class User(val name: String, val age: Int)
来源：http://hz.chenjidiqi.icu/gtmkchicpu.html

[T09] Kotlin：扩展函数
来源：http://hz.guowangkeji.top/gtuptrdnvw.html

fun String.exclaim() = this + "!"
来源：http://hz.wangdashe.top/gtvwbqtjfr.html

[T10] Kotlin：默认参数
来源：http://hz.yuanzhike.top/gtydolpdan.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zdqjudy.top/gtosuydfxx.html

[T11] Kotlin：协程
来源：http://hz.havefunace.top/gtigjahweg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.havefunace.top/gtgcptehpd.html

[T12] Kotlin：解构声明
来源：http://hz.ydzc1.top/gtfbcelwam.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuetiantiany.cn/gtbbwiehdo.html

[T13] Kotlin：只读 Map
来源：http://hz.sysykeji.top/gtnalhlwno.html

val m = mapOf("a" to 1)
来源：http://hz.iojbl.cn/gtewzeqoli.html

[T14] Kotlin：循环
来源：http://hz.xziqi.cn/gtkonvwdjr.html

for (i in 1..10) println(i)
来源：http://hz.hammf.cn/gtayxpqybc.html

[T15] Kotlin：接口
来源：http://hz.wangdashe.top/gtskpybpxa.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtjayrdiac.html

[T16] Swift：Hello World
来源：http://hz.ppjwa.cn/gtggcxjxag.html

print("Hello")
来源：http://hz.xylfe.cn/gtwkfhetma.html

[T17] Swift：变量与常量
来源：http://hz.sxryk.cn/gtskskidpu.html

var a = 1;  let b = 2
来源：http://hz.ybcxt.top/gtsyfnzfwd.html

[T18] Swift：字符串插值
来源：http://hz.dianchejie.cn/gtaqknbgix.html

"值: \(b)"
来源：http://hz.meibo888.top/gtlbszmdxk.html

[T19] Swift：可选绑定
来源：http://hz.zdqjudy.top/gtwcgtqlzo.html

if let n = opt { print(n) }
来源：http://hz.quarkkingdee.top/gtjfpegigj.html

[T20] Swift：数组操作
来源：http://hz.ybcxt.top/gtpbeqlufe.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guowangkeji.top/gtdqtbgzyk.html

[T21] Swift：遍历
来源：http://hz.birdmap.top/gtdewuktfp.html

for x in a { print(x) }
来源：http://hz.gaohongyu789.top/gtzpggjvls.html

[T22] Swift：字典
来源：http://hz.jiagoushi.top/gtkffafvyv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xylfe.cn/gtlfcaszut.html


<!-- 参考信息 -->