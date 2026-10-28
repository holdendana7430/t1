代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hz.feifeiyinyue.top/gtnjdztqcy.html

[R18] 遍历数组
来源：http://hz.jqgfzy.top/gtxpchmhvh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gtorcftklb.html

[R19] 数组长度
来源：http://hz.nwbrower.top/gthgqhpisl.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtnzekljqe.html

[R20] 关联数组（字典）
来源：http://hz.ppjwa.cn/gtxquvluzx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangtech.top/gtfpuwphta.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtvcrdktrz.html

echo "${#s}"
来源：http://hz.yj20258.top/gtfufgdiou.html

[R22] 截取子串
来源：http://hz.yj202588.top/gtyiltbzmm.html

echo "${s:0:5}"
来源：http://hz.iojbl.cn/gtyoxykvfb.html

[R23] 字符串替换
来源：http://hz.birdmap.top/gtmwpptpvg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hongshengwenyu.top/gttgosuyxu.html

[R24] 大小写转换
来源：http://hz.xinyue.icu/gtrobjtuua.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.svipenyu.cn/gtqxcamoxe.html

[R25] 去后缀 / 去前缀
来源：http://hz.cucudq.cn/gtntiatwbi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258888.top/gtxeppvceb.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gthhyaghwp.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxuanxn.top/gtvbejounj.html

[R27] 算术展开
来源：http://hz.zhixingplan.top/gtzjwzmlyl.html

echo $((1 + 2 * 3))
来源：http://hz.chenzaomai.com/gtdzhrijge.html

[R28] 浮点运算
来源：http://hz.jlsjyb.cn/gtyyejaqnw.html

echo "scale=2; 10/3" | bc
来源：http://hz.9152youxi.cn/gtdximduqr.html

[R29] 定义函数
来源：http://hz.svipenyu.cn/gtwnzaysdy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guowangkeji.top/gtxmeexgrd.html

[R30] 函数返回状态码
来源：http://hz.ydzc1.top/gtkkwtcmks.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cucudq.cn/gtzqecqxlc.html

[R31] 局部变量
来源：http://hz.ydjk.org.cn/gtkdpksqsw.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtselbxsak.html

[R32] 参数个数校验
来源：http://hz.chenlongwang.top/gtstnhcccz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhaomingkeji.xyz/gtkhlkftta.html

[R33] 捕获错误并提示行号
来源：http://hz.ppjwa.cn/gtzpwgzeip.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.haohaochexian.top/gtuailqatt.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gteipufkyr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtesifyjkp.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gtbeqknaoj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtenpgobmn.html

[R36] 并发执行多个任务
来源：http://hz.guannengcc.top/gtdvhpxznb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fengsongda.top/gtszfutdti.html

[R37] 把输出赋给变量
来源：http://hz.hnxiangtu.top/gtguoruqng.html

files=$(ls -1)
来源：http://hz.xinyue.icu/gtpctbilnx.html

[R38] 管道串联
来源：http://hz.hnqzz.top/gtlnjjhgjb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtfgrmsoym.html

[R39] 重定向标准输出与错误
来源：http://hz.jyoumei.cn/gtcgkvplna.html

cmd > out.log 2>&1
来源：http://hz.shzxlz.cn/gtprczpxux.html

[R40] 追加写日志
来源：http://hz.jlsjyb.cn/gtulwrwzcg.html

echo "log" >> out.log
来源：http://hz.9152youxi.cn/gtxemaghul.html

[R41] 丢弃输出
来源：http://hz.zdqjudy.top/gtmaswuwpx.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtqxbsyblk.html

[R42] 输入重定向
来源：http://hz.shanyushiyangtech.top/gtbjvpuntd.html

wc -l < a.txt
来源：http://hz.yj20258888.top/gtntimquoq.html

[R43] 按名字查找文件
来源：http://hz.tianlin.xyz/gtktwewlur.html

find . -name "*.log" -type f
来源：http://hz.redwolf501.top/gtgthnpaan.html

[R44] 按修改时间查找
来源：http://hz.quarkkingdee.top/gtxhnlookj.html

find . -mtime -7 -type f
来源：http://hz.feifeiyinyue.top/gtfnwudplu.html

[R45] 批量删除
来源：http://hz.dashuyun.cn/gtyvvzdtod.html

find . -name "*.tmp" -delete
来源：http://hz.zhaomingkeji.xyz/gtkkefvdtw.html

[R46] 递归替换文件内容
来源：http://hz.xingfuxueyuan.xyz/gtuahndsbg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gotoacloud.top/gtrxmodszw.html

[R47] sed 单行替换
来源：http://hz.xuetiantiany.cn/gtlzwdaydf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhaomingkeji.xyz/gtmfjhxfuu.html

[R48] awk 取指定列
来源：http://hz.zhongyouzk.top/gtofyukqgc.html

awk '{print $1, $3}' a.txt
来源：http://hz.tanke756.top/gtgskbutfe.html

[R49] awk 带条件
来源：http://hz.sweek.top/gtbtkwsqcb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guowangkeji.top/gtsneshkvo.html

[R50] awk 求和
来源：http://hz.gaohongyu789.top/gtjnidfzpv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenzaomai.com/gtzvsroeqq.html

[R51] 排序去重取前几
来源：http://hz.fzhhl.top/gtznoeegzm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgufenzy.top/gtnuuceybe.html

[R52] 统计行数
来源：http://hz.yvedp.cn/gtilesjnfl.html

wc -l a.txt
来源：http://hz.snrcjt.cn/gtpgstrlcs.html

[R53] 查看文件头与实时尾
来源：http://hz.zhongyouzk.top/gtxxthwhau.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aibaodan.cn/gtvjjdfkxy.html

[R54] 比较两个文件
来源：http://hz.chenjidiqi.icu/gtkcbldqkc.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtkcnearai.html

[R55] 压缩与解压
来源：http://hz.wangdashe.top/gtoqrqtqdo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.vqdsnc.cn/gtrcmipeci.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtoymkaevx.html

scp file user@host:/path/
来源：http://hz.mhx1999.top/gthjvqotlq.html

[R57] 远程执行命令
来源：http://hz.andypj.xyz/gtjmqrgghm.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gtzkxonzjx.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gtywxqcajw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.snrcjt.cn/gtvmhgjkcy.html

[R59] 发 POST JSON
来源：http://hz.nwbrower.top/gtnbpfzsrn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhixingplan.top/gtxmemlutd.html

[R60] 只看 HTTP 状态码
来源：http://hz.yuanzhike.top/gtwzpkfofv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhaomingkeji.xyz/gtptjyxsel.html

[R61] 磁盘占用
来源：http://hz.aizwys.cn/gtdwltyvmq.html

df -h;  du -sh *
来源：http://hz.jqgufenzy.top/gtddxnqfmy.html

[R62] 找最占空间的文件
来源：http://hz.ydzc1.top/gtwgllvdwu.html

du -ah . | sort -rh | head -10
来源：http://hz.jlsjyb.cn/gtuejtiyvw.html

[R63] 内存与进程
来源：http://hz.cucudq.cn/gtllmaxubm.html

free -h;  ps aux | grep nginx
来源：http://hz.yonumen.top/gtpvmstpyk.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtjyxknpgr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yueranfly.top/gtprfxflsr.html

[R65] 查看端口占用
来源：http://hz.ydzc1.top/gtwqmzdugx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gotoacloud.top/gtdsqcbbpr.html

[R66] 定时任务
来源：http://hz.xingfuxueyuan.xyz/gtwwngoexk.html

crontab -e;  crontab -l
来源：http://hz.ehwqpu.com/gtpnnnxygq.html

[R67] 生成随机十六进制串
来源：http://hz.birdmap.top/gtzzicraoo.html

openssl rand -hex 16
来源：http://hz.feifeiyinyue.top/gtuocriixc.html

[R68] 计算文件校验值
来源：http://hz.yvedp.cn/gthabtuggz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.wangshuangyany.cn/gtujogumad.html

[R69] 生成随机密码
来源：http://hz.dianchejie.cn/gtobtxtuld.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhoulong.xyz/gtdkzpkymo.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gttqmhqirx.html

date +%s;  date -d @1700000000
来源：http://hz.tian-w.cn/gtjsaojmog.html

[R71] 日期格式化
来源：http://hz.bjfxy.top/gtklsvrmbi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtkypqclbm.html

[R72] 等待端口就绪
来源：http://hz.xylfe.cn/gtushazmlv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtstlcjpms.html

[R73] 分割大日志
来源：http://hz.316326.xyz/gttlhmidhq.html

split -l 1000 big.log part_
来源：http://hz.guowangkeji.top/gtugadkuox.html

[R74] 批量重命名
来源：http://hz.birdmap.top/gtdqznbmsx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nwbrower.top/gtjjhrbdyq.html

[R75] 导出环境变量
来源：http://hz.smart0.xyz/gtoyzwfoxo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ybcxt.top/gtfrcgkxbu.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtnzatpxpu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gtjtezgzmz.html

[R77] 读取用户输入
来源：http://hz.sysykeji.top/gtauowgkbw.html

read -rp "请输入: " ans
来源：http://hz.yanxiufei.cn/gtnwkgrkbl.html

[R78] 交互式菜单
来源：http://hz.xziqi.cn/gtnunlvqrg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.meibo888.top/gtmakvqlne.html

[R79] 解析命令行选项
来源：http://hz.zhongyouzk.top/gttgctyycm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydzc1.top/gtvnbosvoc.html

[R80] 查看脚本执行耗时
来源：http://hz.xuanzx.com/gtydhedgrb.html

time ./run.sh
来源：http://hz.chenlongwang.top/gtpqvubfur.html

================================================================================
来源：http://hz.gogol.net.cn/gtukenrjeb.html

S. C / C++ 专题
来源：http://hz.zhijiandao.cn/gtnpnpxocl.html

================================================================================
来源：http://hz.yj20258.top/gtgaxpxbbf.html

[S01] C：Hello World
来源：http://hz.tian-w.cn/gtdcdgqhlo.html

#include <stdio.h>
来源：http://hz.ppjwa.cn/gtswzrgtyb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xingfuxueyuan.xyz/gtcpjkfkih.html

[S02] C：变量与格式化输出
来源：http://hz.iojbl.cn/gtrurodhfx.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhiwuduotai.top/gtmfwwzzze.html

[S03] C：读入整数
来源：http://hz.jinqigufen.top/gtbhqkeugn.html

int x; scanf("%d", &x);
来源：http://hz.jinqigfzy.top/gtwmzitbgz.html

[S04] C：字符串复制
来源：http://hz.gogol.net.cn/gtviyzigqk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangdashe.top/gtlcijjlry.html

[S05] C：字符串长度
来源：http://hz.sufxvd.cn/gtdoaqqmgx.html

strlen(s)
来源：http://hz.cucudq.cn/gttmeawule.html

[S06] C：字符串比较
来源：http://hz.chenjidiqi.icu/gtzqewirkq.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtpanstjhn.html

[S07] C：数组遍历求和
来源：http://hz.ywan-chungtsiang.top/gtqjavhvhs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gtvdbbyddo.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gtaywmxzim.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.havefunace.top/gtruhultoa.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgfzy.top/gtgckrvjqb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.9152youxi.cn/gtuttmgvyk.html

[S10] C：指针与解引用
来源：http://hz.snrcjt.cn/gtqkndsbrr.html

int *p = &a;  *p = 5;
来源：http://hz.jiagoushi.top/gtujoyllfv.html

[S11] C：逐行读文件
来源：http://hz.shuidangran.top/gtapiomrgx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258888.top/gtrswantxm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.vqdsnc.cn/gtzrmgdhvp.html

fclose(f);
来源：http://hz.hysaishi.cn/gtxxnhwaxu.html

[S12] C：写文件
来源：http://hz.zycfv.cn/gtwzbjxssb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhijiandao.cn/gtnswirkpv.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtjkcfbuvn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzhubu.top/gtqezvbzmp.html

[S14] C：枚举
来源：http://hz.sysykeji.top/gtdfbcbvuv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ybcxt.top/gttpbvhvmb.html

[S15] C：类型转换
来源：http://hz.iojbl.cn/gtfazzlzlo.html

(double) a / b
来源：http://hz.hnxiangtu.top/gtcejhotkz.html

[S16] C：位操作置位
来源：http://hz.fengsongda.top/gtitshgnpx.html

x |= (1 << 3);
来源：http://hz.hysaishi.cn/gtxsimyyvd.html

[S17] C：安全拼接字符串
来源：http://hz.0kj1m.cn/gtovsohwcv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.tanke756.top/gtmngdgijl.html

[S18] C：命令行参数
来源：http://hz.jinqigufen.top/gtdmzfgzjz.html

int main(int argc, char **argv)
来源：http://hz.chenlongwang.top/gtsgnbvupf.html

[S19] C：快速排序
来源：http://hz.haohaochexian.top/gtwgmyryux.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtjwmcipyh.html

[S20] C：二分查找
来源：http://hz.wangshuangyany.cn/gtpdlzupin.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtdjyufwzi.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtqcfxbjwv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gthnxuleht.html

[S22] C：字符串转数字
来源：http://hz.52xcode.cn/gtvltgvbum.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.0kj1m.cn/gtqvjafxmd.html

[S23] C：随机数
来源：http://hz.guannengcc.top/gtwirruwev.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtihuwsikh.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gtuyaxwxel.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydjk.org.cn/gtvmfvdylh.html

[S25] C：内存拷贝
来源：http://hz.aizwys.cn/gtinrppagd.html

memcpy(dst, src, n);
来源：http://hz.iojbl.cn/gttblimhre.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtdhfuuldy.html

memset(a, 0, sizeof a);
来源：http://hz.nanxuanxn.top/gtlhqwjcsk.html

[S27] C：定义常量
来源：http://hz.cqqwz.cn/gtevhyiwmq.html

const double PI = 3.14159;
来源：http://hz.xziqi.cn/gtalmfmlih.html

[S28] C：静态变量
来源：http://hz.pycfn.com/gtqzerngta.html

static int counter = 0;
来源：http://hz.hammf.cn/gtprskpohp.html

[S29] C：变参函数
来源：http://hz.hnxiangtu.top/gtwfljwjcc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenjidiqi.icu/gtubxeulnt.html

[S30] C：头文件保护
来源：http://hz.gzhubu.top/gtnvezzcos.html

#ifndef X_H
来源：http://hz.sweek.top/gtxgshwgth.html

#define X_H
来源：http://hz.wangdashe.top/gtdhorrzad.html

#endif
来源：http://hz.tianlin.xyz/gtrjctmjsz.html

[S31] C++：Hello World
来源：http://hz.xuanzx.com/gtalsmojor.html

#include <iostream>
来源：http://hz.gotoacloud.top/gtglllzgod.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sysykeji.top/gthbmjlrnu.html

[S32] C++：字符串
来源：http://hz.yueranfly.top/gtuspxmtjo.html

std::string s = "hi";  s += "!";
来源：http://hz.316326.xyz/gtsvfewhzg.html

[S33] C++：vector 增删
来源：http://hz.316326.xyz/gttvdazrbu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtdimxfrju.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtkhswulym.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shangyingyoupin.top/gtcapayrez.html

[S35] C++：map
来源：http://hz.iojbl.cn/gtfpemlrws.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ppjwa.cn/gtjtbmgzmn.html

[S36] C++：unordered_map
来源：http://hz.yonumen.top/gtdeaqcudz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtiyydnozb.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtebxrkazh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgfzy.top/gtprlwzrea.html

[S38] C++：排序
来源：http://hz.nanxuanxn.top/gtjoynclib.html

std::sort(v.begin(), v.end());
来源：http://hz.tianlin.xyz/gtzhlektfj.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtebdflddt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangkeji.top/gtggsbjqve.html

[S40] C++：查找元素
来源：http://hz.xingfuxueyuan.xyz/gtkujdhyat.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ywan-chungtsiang.top/gthxhdmihw.html

[S41] C++：类与构造函数
来源：http://hz.meibo888.top/gtslelgflj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.andypj.xyz/gtwnomzzuz.html

[S42] C++：继承与虚函数
来源：http://hz.jyoumei.cn/gthlcyjdlw.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtfsakuzvh.html

[S43] C++：智能指针
来源：http://hz.vqdsnc.cn/gthudyikfe.html

auto p = std::make_unique<int>(5);
来源：http://hz.xylfe.cn/gtohhqahhf.html

[S44] C++：引用传参
来源：http://hz.vqdsnc.cn/gtmdqdrttd.html

void inc(int &x) { ++x; }
来源：http://hz.zhengqikj.top/gtfiofrnaf.html

[S45] C++：lambda
来源：http://hz.yangfankeji.com/gtjeellwaf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jlsjyb.cn/gtolwhxtxf.html

[S46] C++：函数模板
来源：http://hz.daria6918.cn/gtawisykta.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guannengcc.top/gtlyfureid.html

[S47] C++：结构化绑定遍历
来源：http://hz.havefunace.top/gtdlussaxu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gzhubu.top/gtnqjiyeob.html

[S48] C++：逐行读文件
来源：http://hz.ybcxt.top/gtcrbdenwp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yongpay.top/gttjhcfqsc.html

while (std::getline(in, line)) { }
来源：http://hz.snrcjt.cn/gtezuccoga.html

[S49] C++：写文件
来源：http://hz.jiagoushi.top/gtifxwkcwk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hfpthk.cn/gtiqiaxjug.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gtgdahpbwd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yanxiufei.cn/gtkjqdgedx.html

[S51] C++：显式类型转换
来源：http://hz.jianghu66.top/gtstalwbhu.html

static_cast<double>(a) / b
来源：http://hz.zhaomingkeji.xyz/gtdfsckmpy.html

[S52] C++：const 与 noexcept
来源：http://hz.pycfn.com/gtynazazfq.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangtech.top/gtifvnquvh.html

[S53] C++：移动语义
来源：http://hz.snrcjt.cn/gtcmxlykga.html

std::vector<int> w = std::move(v);
来源：http://hz.meibo888.top/gtpbwruitu.html

[S54] C++：异常处理
来源：http://hz.cqqwz.cn/gtwuinuvhc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hysaishi.cn/gtxyohtvky.html

[S55] C++：结构化绑定
来源：http://hz.zycfv.cn/gtfgdickyg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shangyingyoupin.top/gtbqdqznsd.html

[S56] C++：optional
来源：http://hz.hywenlv.cn/gtdpqpfzbc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangtech.top/gthpdvgkuq.html

[S57] C++：编译期常量
来源：http://hz.wangshuangyany.cn/gtydpmhucb.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gtztetpteh.html

[S58] C++：命名空间
来源：http://hz.jyoumei.cn/gtllnqyvup.html

namespace ns { int f() { return 1; } }
来源：http://hz.shuidangran.top/gtlegoyvhm.html

[S59] C++：静态断言
来源：http://hz.nanxuanxn.top/gtvlfypozs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuetiantiany.cn/gtjaemfgqa.html

[S60] C++：遍历并删除元素
来源：http://hz.aizwys.cn/gtguxacesl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aibaodan.cn/gttoacunyi.html

================================================================================
来源：http://hz.xuanzx.com/gtfjnmmyje.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtmdtbqmbv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxkvkshqk.html

[T01] Kotlin：Hello World
来源：http://hz.ivvv.top/gtgmbdsjyi.html

println("Hello")
来源：http://hz.sysykeji.top/gtecqfqcga.html

[T02] Kotlin：变量
来源：http://hz.dianchejie.cn/gthdpaeiss.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sxryk.cn/gtjmjgowcx.html

[T03] Kotlin：字符串模板
来源：http://hz.9152youxi.cn/gtlmtovwlb.html

"值: $b"
来源：http://hz.cucudq.cn/gttkxoueom.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gtkxezwqjc.html

val n: String? = null;  n?.length
来源：http://hz.zycfv.cn/gtapqloceb.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gtryebbfah.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.haohaochexian.top/gtfqmgnozb.html

[T06] Kotlin：集合映射
来源：http://hz.shangyingyoupin.top/gtserynzeq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hywenlv.cn/gtnniqfocu.html

[T07] Kotlin：集合过滤
来源：http://hz.chenzaomai.com/gtnltokqvo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gaohongyu789.top/gtultwzqde.html

[T08] Kotlin：数据类
来源：http://hz.0kj1m.cn/gttovgsjvl.html

data class User(val name: String, val age: Int)
来源：http://hz.cheryme.top/gtsciulayw.html

[T09] Kotlin：扩展函数
来源：http://hz.fzhhl.top/gtepakspwj.html

fun String.exclaim() = this + "!"
来源：http://hz.chenzaomai.com/gtzfjwmuyd.html

[T10] Kotlin：默认参数
来源：http://hz.xylfe.cn/gtyyszelbt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtenuzlbyc.html

[T11] Kotlin：协程
来源：http://hz.52xcode.cn/gtsphenley.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.andypj.xyz/gtgoxvshhr.html

[T12] Kotlin：解构声明
来源：http://hz.zhongyouzk.top/gtjkqhsipe.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhoulong.xyz/gtqpgyopbx.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gtvbvdpklu.html

val m = mapOf("a" to 1)
来源：http://hz.xylfe.cn/gtmeixbswj.html

[T14] Kotlin：循环
来源：http://hz.jianghu66.top/gtcjtyvimd.html

for (i in 1..10) println(i)
来源：http://hz.xinyue.icu/gtvvxdlyoc.html

[T15] Kotlin：接口
来源：http://hz.yangfankeji.com/gtgsrxdexe.html

interface Shape { fun area(): Double }
来源：http://hz.sysykeji.top/gtbirkynes.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gtiwzrusbh.html

print("Hello")
来源：http://hz.redwolf501.top/gtwcmhaueu.html

[T17] Swift：变量与常量
来源：http://hz.ywan-chungtsiang.top/gtqfgagpdf.html

var a = 1;  let b = 2
来源：http://hz.yanxiufei.cn/gtkmqeqcoa.html

[T18] Swift：字符串插值
来源：http://hz.0kj1m.cn/gtcjrkvflq.html

"值: \(b)"
来源：http://hz.dashuyun.cn/gtyboaolks.html

[T19] Swift：可选绑定
来源：http://hz.ywan-chungtsiang.top/gtmtikcdml.html

if let n = opt { print(n) }
来源：http://hz.xuanzx.com/gtjhqtmqld.html

[T20] Swift：数组操作
来源：http://hz.sxryk.cn/gtlrbegygs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhijiandao.cn/gtpgavbbkc.html


<!-- 参考信息 -->