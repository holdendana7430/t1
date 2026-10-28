代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guowangkeji.top/gtxrvhgfut.html

[R18] 遍历数组
来源：http://hz.yonumen.top/gtuttzijfo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.iojbl.cn/gtutcmplqc.html

[R19] 数组长度
来源：http://hz.guannengcc.top/gtunakeqkv.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtwajqeeil.html

[R20] 关联数组（字典）
来源：http://hz.daxiang520.top/gtfevfztrt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hongshengwenyu.top/gtakanrzix.html

[R21] 字符串长度
来源：http://hz.yueranfly.top/gtppzkowll.html

echo "${#s}"
来源：http://hz.dianchejie.cn/gtrnbtrahu.html

[R22] 截取子串
来源：http://hz.cashguo.top/gtlxeydeyx.html

echo "${s:0:5}"
来源：http://hz.ehwqpu.com/gtgrwcdibz.html

[R23] 字符串替换
来源：http://hz.ydzc1.top/gtxzphswvm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nwbrower.top/gttxttoobz.html

[R24] 大小写转换
来源：http://hz.guowangkeji.top/gtkjrcmqmp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tian-w.cn/gtinwartna.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuxming.cn/gtqdaikuej.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yongpay.top/gtzxyqdmmd.html

[R26] 命令替换
来源：http://hz.c1oappe.top/gtdxmzmodm.html

now=$(date +%F); echo "$now"
来源：http://hz.xingfuxueyuan.xyz/gteaahrgfq.html

[R27] 算术展开
来源：http://hz.quarkkingdee.top/gtcvfprejo.html

echo $((1 + 2 * 3))
来源：http://hz.jqgfzy.top/gtvhecyfoc.html

[R28] 浮点运算
来源：http://hz.hammf.cn/gtngxdjpob.html

echo "scale=2; 10/3" | bc
来源：http://hz.c1oappe.top/gtkqmtxveo.html

[R29] 定义函数
来源：http://hz.chenzaomai.com/gtavubbchf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xziqi.cn/gtwhcnvpzz.html

[R30] 函数返回状态码
来源：http://hz.zhijiandao.cn/gtjzqoycyd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.mhx1999.top/gtfgttgtpm.html

[R31] 局部变量
来源：http://hz.gaohongyu789.top/gttsqaunmp.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenzaomai.com/gtibesejut.html

[R32] 参数个数校验
来源：http://hz.xinyue.icu/gtkqozevju.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtxncgyexo.html

[R33] 捕获错误并提示行号
来源：http://hz.yongpay.top/gtpiaairzv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtviqlneud.html

[R34] 退出时清理
来源：http://hz.zdqjudy.top/gtpvytceyn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtddtjwaan.html

[R35] 后台执行并等待
来源：http://hz.xuanzx.com/gtxnlwjomk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hongshengwenyu.top/gtwwtsthng.html

[R36] 并发执行多个任务
来源：http://hz.yuanzhike.top/gthcvmwnaa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.52xcode.cn/gtcccuuuxo.html

[R37] 把输出赋给变量
来源：http://hz.fengsongda.top/gtcfcpxaod.html

files=$(ls -1)
来源：http://hz.gaohongyu789.top/gtgfypyewx.html

[R38] 管道串联
来源：http://hz.jiagoushi.top/gtfwzmmbqx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtpxawdnba.html

[R39] 重定向标准输出与错误
来源：http://hz.nwbrower.top/gtqbdpexfn.html

cmd > out.log 2>&1
来源：http://hz.zhengqikj.top/gtklulnven.html

[R40] 追加写日志
来源：http://hz.c1oappe.top/gtjfksvncv.html

echo "log" >> out.log
来源：http://hz.daria6918.cn/gtghcapibg.html

[R41] 丢弃输出
来源：http://hz.yongpay.top/gtkfzedksg.html

cmd >/dev/null 2>&1
来源：http://hz.0kj1m.cn/gtalqdjuzo.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gtiztkjifx.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gtuuszowfo.html

[R43] 按名字查找文件
来源：http://hz.daria6918.cn/gtmjauuhww.html

find . -name "*.log" -type f
来源：http://hz.yueranfly.top/gthobxnach.html

[R44] 按修改时间查找
来源：http://hz.yonumen.top/gtooqftqlw.html

find . -mtime -7 -type f
来源：http://hz.zhijiandao.cn/gtylzynxgz.html

[R45] 批量删除
来源：http://hz.aizwys.cn/gtzxsezbdy.html

find . -name "*.tmp" -delete
来源：http://hz.gotoacloud.top/gtkgzlqspx.html

[R46] 递归替换文件内容
来源：http://hz.jiagoushi.top/gtqgjwopeo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtzsapkbah.html

[R47] sed 单行替换
来源：http://hz.yuxming.cn/gtwirnlvgm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yanxiufei.cn/gtwzqvvipp.html

[R48] awk 取指定列
来源：http://hz.zhixingplan.top/gtvrcjvabk.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuanzx.com/gtjwxovkkj.html

[R49] awk 带条件
来源：http://hz.hysaishi.cn/gthlhsvpqd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gotoacloud.top/gtsqqplkle.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtvpdwqxsd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gzhubu.top/gtfvfozkzt.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gtpjlekbnw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xziqi.cn/gtwqaujyro.html

[R52] 统计行数
来源：http://hz.jqgufenzy.top/gtbqwkrukn.html

wc -l a.txt
来源：http://hz.birdmap.top/gtuamuonhg.html

[R53] 查看文件头与实时尾
来源：http://hz.snrcjt.cn/gtnbijwsum.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtjqgsszbp.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtwsfqksqx.html

diff a.txt b.txt
来源：http://hz.tian-w.cn/gtsvzovqnh.html

[R55] 压缩与解压
来源：http://hz.cashguo.top/gtjginrrwk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cheryme.top/gtttbmwmog.html

[R56] 远程拷贝
来源：http://hz.sweek.top/gtocjrpfju.html

scp file user@host:/path/
来源：http://hz.gzhubu.top/gtivlbqjur.html

[R57] 远程执行命令
来源：http://hz.nanxinkj.top/gtbyipqorv.html

ssh user@host 'uptime'
来源：http://hz.gzhubu.top/gtnycgsolk.html

[R58] 下载文件
来源：http://hz.zhengqikj.top/gtlrkgfhnj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtukqnndwe.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtvmtgyibh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtzeggbiwq.html

[R60] 只看 HTTP 状态码
来源：http://hz.hywenlv.cn/gtimtekuuu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.316326.xyz/gticujwfik.html

[R61] 磁盘占用
来源：http://hz.jinqigfzy.top/gtuoxtbewy.html

df -h;  du -sh *
来源：http://hz.zhoulong.xyz/gtnagtahuk.html

[R62] 找最占空间的文件
来源：http://hz.pycfn.com/gtxepzqnux.html

du -ah . | sort -rh | head -10
来源：http://hz.chenzaomai.com/gtqejobljb.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gtqgcsglas.html

free -h;  ps aux | grep nginx
来源：http://hz.andypj.xyz/gthixgzlfh.html

[R64] 结束进程
来源：http://hz.meibo888.top/gtjzhbwlbv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenzaomai.com/gtsfbmamdn.html

[R65] 查看端口占用
来源：http://hz.hnxiangtu.top/gtjrnktlhn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sweek.top/gtuuttvxlm.html

[R66] 定时任务
来源：http://hz.iojbl.cn/gtlyskzile.html

crontab -e;  crontab -l
来源：http://hz.yueranfly.top/gtjpdbnetu.html

[R67] 生成随机十六进制串
来源：http://hz.ybcxt.top/gtrsfurfdu.html

openssl rand -hex 16
来源：http://hz.svipenyu.cn/gtliijipih.html

[R68] 计算文件校验值
来源：http://hz.gaohongyu789.top/gtajblrkfb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhixingplan.top/gtmtmflkyr.html

[R69] 生成随机密码
来源：http://hz.andypj.xyz/gtuidvskwz.html

head -c 16 /dev/urandom | base64
来源：http://hz.pycfn.com/gteyhcndgf.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtsjdeaznf.html

date +%s;  date -d @1700000000
来源：http://hz.sufxvd.cn/gteimvwaal.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gtdeiawgga.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cheryme.top/gtfjzmrgiw.html

[R72] 等待端口就绪
来源：http://hz.zhengqikj.top/gtfaysexgk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tian-w.cn/gtxbdcruvz.html

[R73] 分割大日志
来源：http://hz.aizwys.cn/gtnkombxon.html

split -l 1000 big.log part_
来源：http://hz.chenzaomai.com/gtpcitouyj.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gtjyxxwlwz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ybcxt.top/gtgkovaaow.html

[R75] 导出环境变量
来源：http://hz.ydzc1.top/gtodypordo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.smart0.xyz/gtclutpjto.html

[R76] 使用临时文件
来源：http://hz.fengsongda.top/gtcvbrrwwr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gtjrrpsoiz.html

[R77] 读取用户输入
来源：http://hz.hysaishi.cn/gtisdgefut.html

read -rp "请输入: " ans
来源：http://hz.xylfe.cn/gtxnclxpyx.html

[R78] 交互式菜单
来源：http://hz.havefunace.top/gtgkszttan.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guowangkeji.top/gttdxcyjcm.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtqunpsbvs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj202588.top/gtozlsdnpc.html

[R80] 查看脚本执行耗时
来源：http://hz.iojbl.cn/gtgpizykbq.html

time ./run.sh
来源：http://hz.yj20258.top/gthmazidvl.html

================================================================================
来源：http://hz.guannengcc.top/gtppynevlw.html

S. C / C++ 专题
来源：http://hz.yanxiufei.cn/gtkglwescz.html

================================================================================
来源：http://hz.sufxvd.cn/gteoiezkeg.html

[S01] C：Hello World
来源：http://hz.shzxlz.cn/gtczfwewje.html

#include <stdio.h>
来源：http://hz.mhx1999.top/gteeemvtzt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hfpthk.cn/gtwupudbpk.html

[S02] C：变量与格式化输出
来源：http://hz.kuanghao11.cn/gtyvclruwq.html

int a = 10; printf("%d\n", a);
来源：http://hz.dianchejie.cn/gtshdnlvkc.html

[S03] C：读入整数
来源：http://hz.yvedp.cn/gtnztjmxhb.html

int x; scanf("%d", &x);
来源：http://hz.yuanzhike.top/gtetsiouuk.html

[S04] C：字符串复制
来源：http://hz.smart0.xyz/gttfamgyju.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.0kj1m.cn/gtnknmrnoe.html

[S05] C：字符串长度
来源：http://hz.tianlin.xyz/gtxjovgbtb.html

strlen(s)
来源：http://hz.tian-w.cn/gtxmeqoaps.html

[S06] C：字符串比较
来源：http://hz.iojbl.cn/gthtjhzvnd.html

strcmp(a, b) == 0
来源：http://hz.ydzc1.top/gtydsxuqbd.html

[S07] C：数组遍历求和
来源：http://hz.jiagoushi.top/gtrqabnnzq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cucudq.cn/gtpxasyzkv.html

[S08] C：动态内存分配与释放
来源：http://hz.quarkkingdee.top/gtpvgspivc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtziotiszc.html

[S09] C：结构体定义与初始化
来源：http://hz.aizwys.cn/gtzaflmmdn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sysykeji.top/gtzisfrotp.html

[S10] C：指针与解引用
来源：http://hz.pengpengdd.cyou/gtrzdrtrtw.html

int *p = &a;  *p = 5;
来源：http://hz.redwolf501.top/gtsbmompdw.html

[S11] C：逐行读文件
来源：http://hz.pycfn.com/gtrjfcehno.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtunawppmz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cdnleiting.top/gtzgeepwrs.html

fclose(f);
来源：http://hz.sxryk.cn/gtpajsyiqy.html

[S12] C：写文件
来源：http://hz.gotoacloud.top/gttzbxghpd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhiwuduotai.top/gttjfqyada.html

[S13] C：宏定义
来源：http://hz.zhengqikj.top/gtlbxlkuyu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xinyue.icu/gtreoozaep.html

[S14] C：枚举
来源：http://hz.guannengcc.top/gtuexdoydm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtypvskyqb.html

[S15] C：类型转换
来源：http://hz.gogol.net.cn/gtookfrjfa.html

(double) a / b
来源：http://hz.jiagoushi.top/gtgbrblrhy.html

[S16] C：位操作置位
来源：http://hz.fzhhl.top/gtpnspztdu.html

x |= (1 << 3);
来源：http://hz.gotoacloud.top/gtztalzuhr.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtvdblytmn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sufxvd.cn/gtgaoqqjne.html

[S18] C：命令行参数
来源：http://hz.shzxlz.cn/gtjpbrcvqx.html

int main(int argc, char **argv)
来源：http://hz.gogol.net.cn/gtpisqbjuf.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gtnnphccnv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtsblqqwae.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtqeyadoqi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtuhfhqdoa.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gthbnwmpgg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gaohongyu789.top/gtirregqvc.html

[S22] C：字符串转数字
来源：http://hz.snrcjt.cn/gttfkwpxwu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ppjwa.cn/gtbpctqfjj.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtunlkktwj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zycfv.cn/gtmpihxiwu.html

[S24] C：获取本地时间
来源：http://hz.xuetiantiany.cn/gtzfcgxobj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guowangkeji.top/gthjmcmsjw.html

[S25] C：内存拷贝
来源：http://hz.gogol.net.cn/gtiwosyfsh.html

memcpy(dst, src, n);
来源：http://hz.ywan-chungtsiang.top/gthswlvcan.html

[S26] C：内存清零
来源：http://hz.hnqzz.top/gtevuoakhu.html

memset(a, 0, sizeof a);
来源：http://hz.jianghu66.top/gtkpzwdblx.html

[S27] C：定义常量
来源：http://hz.ydjk.org.cn/gtaqrhisxo.html

const double PI = 3.14159;
来源：http://hz.yj202588.top/gthjneuwgq.html

[S28] C：静态变量
来源：http://hz.tian-w.cn/gtekdtdrvx.html

static int counter = 0;
来源：http://hz.feifeiyinyue.top/gteeernybg.html

[S29] C：变参函数
来源：http://hz.yj202588.top/gtqppswhbq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cheryme.top/gtjzhxswyc.html

[S30] C：头文件保护
来源：http://hz.yvedp.cn/gtkytsmdlc.html

#ifndef X_H
来源：http://hz.zhixingplan.top/gtlrfvneag.html

#define X_H
来源：http://hz.feifeiyinyue.top/gtxcnpkwas.html

#endif
来源：http://hz.ivvv.top/gthhlzqiti.html

[S31] C++：Hello World
来源：http://hz.zhijiandao.cn/gthqfumfra.html

#include <iostream>
来源：http://hz.0kj1m.cn/gtznzzgkev.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aibaodan.cn/gtgtrjypwb.html

[S32] C++：字符串
来源：http://hz.feifeiyinyue.top/gtrgubupve.html

std::string s = "hi";  s += "!";
来源：http://hz.sxryk.cn/gtqfofrilz.html

[S33] C++：vector 增删
来源：http://hz.jinghuilouyu.cn/gttvisgcsx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tian-w.cn/gtxhlihfkg.html

[S34] C++：遍历 vector
来源：http://hz.cucudq.cn/gtbdpcbrgu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gotoacloud.top/gtwgmztctt.html

[S35] C++：map
来源：http://hz.yueranfly.top/gtwsermdim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtuuohzvux.html

[S36] C++：unordered_map
来源：http://hz.svipenyu.cn/gtawdwgnop.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtjymnjfff.html

[S37] C++：set
来源：http://hz.quarkkingdee.top/gtbfwuzmgt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gthtdvbjur.html

[S38] C++：排序
来源：http://hz.gaohongyu789.top/gtwfwrmrcx.html

std::sort(v.begin(), v.end());
来源：http://hz.xinyue.icu/gtitonupgh.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtkehxutsr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yonumen.top/gtimczscpw.html

[S40] C++：查找元素
来源：http://hz.316326.xyz/gtimfkxlsc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gtxrgtnzhh.html

[S41] C++：类与构造函数
来源：http://hz.cashguo.top/gtnwmvkncn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pycfn.com/gtbkmndqrq.html

[S42] C++：继承与虚函数
来源：http://hz.chenlongwang.top/gtlxtvnzoy.html

class B : public Base { public: void f() override {} };
来源：http://hz.c1oappe.top/gtvdijooea.html

[S43] C++：智能指针
来源：http://hz.shangyingyoupin.top/gtqcxlxfdm.html

auto p = std::make_unique<int>(5);
来源：http://hz.xingfuxueyuan.xyz/gtmknaeqbj.html

[S44] C++：引用传参
来源：http://hz.kuanghao11.cn/gtubetcnam.html

void inc(int &x) { ++x; }
来源：http://hz.jinghuilouyu.cn/gtcapcgdip.html

[S45] C++：lambda
来源：http://hz.birdmap.top/gtsmcgitgs.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gttasdpjns.html

[S46] C++：函数模板
来源：http://hz.smart0.xyz/gtnsmgtqzs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guowangkeji.top/gtvivfykkg.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuetiantiany.cn/gtblyiqpga.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhengqikj.top/gtahcqkvop.html

[S48] C++：逐行读文件
来源：http://hz.chenlongwang.top/gtewqsplkl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.guannengcc.top/gtbpggvlbx.html

while (std::getline(in, line)) { }
来源：http://hz.c1oappe.top/gtpusxtwzh.html

[S49] C++：写文件
来源：http://hz.yj20258.top/gtuqvzzkte.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.bjfxy.top/gtxrwhqcqf.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gttmaowrau.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hysaishi.cn/gtlcoswljn.html

[S51] C++：显式类型转换
来源：http://hz.jlsjyb.cn/gtkodmuczy.html

static_cast<double>(a) / b
来源：http://hz.shuidangran.top/gtuhqzptpo.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtmwvnzyky.html

int size() const noexcept { return n_; }
来源：http://hz.nanxinkj.top/gtdyeezsrc.html

[S53] C++：移动语义
来源：http://hz.tianlin.xyz/gtizydbwgm.html

std::vector<int> w = std::move(v);
来源：http://hz.guannengcc.top/gthgsiqyuw.html

[S54] C++：异常处理
来源：http://hz.yuanzhike.top/gtxbbssulr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xingfuxueyuan.xyz/gtyrqfpuni.html

[S55] C++：结构化绑定
来源：http://hz.yanxiufei.cn/gtqwnenfxp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.svipenyu.cn/gtpdxsrjjk.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtefxjzlqk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shangyingyoupin.top/gthefvlzat.html

[S57] C++：编译期常量
来源：http://hz.hfpthk.cn/gtsrsmbmpb.html

constexpr int N = 10;
来源：http://hz.yongpay.top/gtpmyjciep.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtkgkvctwj.html

namespace ns { int f() { return 1; } }
来源：http://hz.cdnleiting.top/gtaoggzxos.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gtzaeswgcu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuanzhike.top/gtppchgvff.html

[S60] C++：遍历并删除元素
来源：http://hz.chenlongwang.top/gtsnlnnndv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.iojbl.cn/gtqkhafrlw.html

================================================================================
来源：http://hz.jiagoushi.top/gtjurvfmkp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gtlthuxqrd.html

================================================================================
来源：http://hz.ydzc1.top/gtjmcmblsy.html

[T01] Kotlin：Hello World
来源：http://hz.xylfe.cn/gtqikovuxf.html

println("Hello")
来源：http://hz.birdmap.top/gtsmyyyxql.html

[T02] Kotlin：变量
来源：http://hz.xylfe.cn/gtewrewwdp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tian-w.cn/gtjwcawwzb.html

[T03] Kotlin：字符串模板
来源：http://hz.havefunace.top/gtpxffrswj.html

"值: $b"
来源：http://hz.iojbl.cn/gttiqnkqsv.html

[T04] Kotlin：空安全
来源：http://hz.yanxiufei.cn/gtkuylucjf.html

val n: String? = null;  n?.length
来源：http://hz.quarkkingdee.top/gtrquvlisr.html

[T05] Kotlin：when 表达式
来源：http://hz.zhixingplan.top/gtdmvvpybn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ppjwa.cn/gtcbiabrud.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtadvztykp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj20258888.top/gtopytitxa.html

[T07] Kotlin：集合过滤
来源：http://hz.hysaishi.cn/gtndpuzcps.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jlsjyb.cn/gtmisupxks.html

[T08] Kotlin：数据类
来源：http://hz.tanke756.top/gtronpwsgb.html

data class User(val name: String, val age: Int)
来源：http://hz.aizwys.cn/gtvhffmnvo.html

[T09] Kotlin：扩展函数
来源：http://hz.pycfn.com/gtsciylkjw.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxinkj.top/gtwruatjou.html

[T10] Kotlin：默认参数
来源：http://hz.dashuyun.cn/gtaxsrsesw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.birdmap.top/gtaawttcge.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gtnwhgeqev.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xziqi.cn/gtuhoyzhuz.html

[T12] Kotlin：解构声明
来源：http://hz.hywenlv.cn/gtlwwqkoam.html

val (a, b) = Pair(1, 2)
来源：http://hz.haohaochexian.top/gthkxstygj.html

[T13] Kotlin：只读 Map
来源：http://hz.xuetiantiany.cn/gtfnurdnpf.html

val m = mapOf("a" to 1)
来源：http://hz.jqgufenzy.top/gtznbrdlfr.html

[T14] Kotlin：循环
来源：http://hz.sweek.top/gtgxbptorn.html

for (i in 1..10) println(i)
来源：http://hz.shangyingyoupin.top/gtcrumnewo.html

[T15] Kotlin：接口
来源：http://hz.hfpthk.cn/gtxrfolinm.html

interface Shape { fun area(): Double }
来源：http://hz.hysaishi.cn/gtmkuwgmav.html

[T16] Swift：Hello World
来源：http://hz.chenjidiqi.icu/gtpwsiahay.html

print("Hello")
来源：http://hz.yangfankeji.com/gtgynllzgd.html

[T17] Swift：变量与常量
来源：http://hz.yvedp.cn/gtfqeydihs.html

var a = 1;  let b = 2
来源：http://hz.havefunace.top/gtbkkqafso.html

[T18] Swift：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtvmtzjlhn.html

"值: \(b)"
来源：http://hz.ehwqpu.com/gtgizdcnud.html

[T19] Swift：可选绑定
来源：http://hz.cheryme.top/gtzukykimk.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtbgdfkbmo.html

[T20] Swift：数组操作
来源：http://hz.sufxvd.cn/gtxjqlmrmc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gtxvhkxuqj.html


<!-- 参考信息 -->