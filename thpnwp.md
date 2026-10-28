代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gtlaoyxdad.html

[R24] 大小写转换
来源：http://hz.hysaishi.cn/gtpeisqsem.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.9152youxi.cn/gtwdtxsawc.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangtech.top/gtcratrmjf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtzgdzcjxw.html

[R26] 命令替换
来源：http://hz.zhiwuduotai.top/gtxaispnbz.html

now=$(date +%F); echo "$now"
来源：http://hz.ppjwa.cn/gtobiyuepy.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtfgkyouic.html

echo $((1 + 2 * 3))
来源：http://hz.sysykeji.top/gtuercgptf.html

[R28] 浮点运算
来源：http://hz.yuanzhike.top/gtiqwqmbjd.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtehoyanmw.html

[R29] 定义函数
来源：http://hz.yvedp.cn/gtzeibpyfz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ehwqpu.com/gtmwnwuyuj.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtpuyizcin.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydzc1.top/gtfvmrlymj.html

[R31] 局部变量
来源：http://hz.chenjidiqi.icu/gtzbejdpdj.html

f() { local x=1; echo "$x"; }
来源：http://hz.birdmap.top/gtenyqmnwd.html

[R32] 参数个数校验
来源：http://hz.hnqzz.top/gtdxsablpr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangdashe.top/gtdmgximtd.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtvxdlebug.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gtpcicswri.html

[R34] 退出时清理
来源：http://hz.yuanzhike.top/gtbuvsngqg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtmpcokqti.html

[R35] 后台执行并等待
来源：http://hz.yj20258888.top/gtogsiojrj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hammf.cn/gtxcwajfjk.html

[R36] 并发执行多个任务
来源：http://hz.vqdsnc.cn/gtxomtakmh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jlsjyb.cn/gtsvxffcyv.html

[R37] 把输出赋给变量
来源：http://hz.guannengcc.top/gtwavwzytw.html

files=$(ls -1)
来源：http://hz.sxryk.cn/gtrhonebmo.html

[R38] 管道串联
来源：http://hz.wangdashe.top/gtiuyoaqdo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuanzhike.top/gtzsodbcer.html

[R39] 重定向标准输出与错误
来源：http://hz.jlsjyb.cn/gtcnuuzpyz.html

cmd > out.log 2>&1
来源：http://hz.hongshengwenyu.top/gtlvbkogno.html

[R40] 追加写日志
来源：http://hz.ppjwa.cn/gtpviuzohy.html

echo "log" >> out.log
来源：http://hz.shzxlz.cn/gtkvbryaqu.html

[R41] 丢弃输出
来源：http://hz.jqgfzy.top/gteudmhdlk.html

cmd >/dev/null 2>&1
来源：http://hz.jiagoushi.top/gtnazsvegm.html

[R42] 输入重定向
来源：http://hz.iojbl.cn/gteakkdpyn.html

wc -l < a.txt
来源：http://hz.havefunace.top/gtjbevdcqp.html

[R43] 按名字查找文件
来源：http://hz.gzhubu.top/gtjsqowcky.html

find . -name "*.log" -type f
来源：http://hz.chenlongwang.top/gthnmzucov.html

[R44] 按修改时间查找
来源：http://hz.0kj1m.cn/gtefznhytl.html

find . -mtime -7 -type f
来源：http://hz.andypj.xyz/gtghvsclhk.html

[R45] 批量删除
来源：http://hz.hfpthk.cn/gtgcyxjogn.html

find . -name "*.tmp" -delete
来源：http://hz.nanxuanxn.top/gtylsynucw.html

[R46] 递归替换文件内容
来源：http://hz.ywan-chungtsiang.top/gtakzyyzxe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jlsjyb.cn/gtlhfigeav.html

[R47] sed 单行替换
来源：http://hz.gotoacloud.top/gtydmxxfop.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shangyingyoupin.top/gtfmvwikdm.html

[R48] awk 取指定列
来源：http://hz.yanxiufei.cn/gtrkjffbki.html

awk '{print $1, $3}' a.txt
来源：http://hz.xinyue.icu/gtehfbouwp.html

[R49] awk 带条件
来源：http://hz.pengpengdd.cyou/gtxvrnixog.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tanke756.top/gtilrlulmt.html

[R50] awk 求和
来源：http://hz.jqgufenzy.top/gtcrhcqili.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cheryme.top/gtcroofeyz.html

[R51] 排序去重取前几
来源：http://hz.iojbl.cn/gtwjpmdhoj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shuidangran.top/gtjudzsfjx.html

[R52] 统计行数
来源：http://hz.nanxuanxn.top/gtknszbrbu.html

wc -l a.txt
来源：http://hz.hnxiangtu.top/gtgdlepkiw.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtgvprzptv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.svipenyu.cn/gteknvvvnb.html

[R54] 比较两个文件
来源：http://hz.guowangkeji.top/gtazwofzfp.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gthjjuvoit.html

[R55] 压缩与解压
来源：http://hz.yangfankeji.com/gtkjcnlexe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sxryk.cn/gtnxpqbpdk.html

[R56] 远程拷贝
来源：http://hz.shangyingyoupin.top/gttdkghyli.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gtmqrldrqw.html

[R57] 远程执行命令
来源：http://hz.cheryme.top/gtftrtcsti.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtdfrzkzdh.html

[R58] 下载文件
来源：http://hz.nwbrower.top/gtldziprsh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhongyouzk.top/gtgquprdkb.html

[R59] 发 POST JSON
来源：http://hz.yuxming.cn/gtxvlbbxtp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtcwybohfa.html

[R60] 只看 HTTP 状态码
来源：http://hz.sysykeji.top/gtlbphjrvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ywan-chungtsiang.top/gtquqvcqck.html

[R61] 磁盘占用
来源：http://hz.yuanzhike.top/gtocnwjgll.html

df -h;  du -sh *
来源：http://hz.ydjk.org.cn/gtbbmrfdfh.html

[R62] 找最占空间的文件
来源：http://hz.zhixingplan.top/gtfhhwrycv.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtfsscupff.html

[R63] 内存与进程
来源：http://hz.guannengcc.top/gtcpczgrqh.html

free -h;  ps aux | grep nginx
来源：http://hz.gaohongyu789.top/gtudiirlif.html

[R64] 结束进程
来源：http://hz.yangfankeji.com/gtpxrkehba.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hywenlv.cn/gtfngsjrxe.html

[R65] 查看端口占用
来源：http://hz.ivvv.top/gtsijuouet.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinghuilouyu.cn/gttpohyely.html

[R66] 定时任务
来源：http://hz.chenlongwang.top/gtzriuaesr.html

crontab -e;  crontab -l
来源：http://hz.andypj.xyz/gttksbrhhx.html

[R67] 生成随机十六进制串
来源：http://hz.xylfe.cn/gtmbhsners.html

openssl rand -hex 16
来源：http://hz.nanxinkj.top/gtpkwzysaf.html

[R68] 计算文件校验值
来源：http://hz.snrcjt.cn/gtrvvdxual.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cqqwz.cn/gthvhpptmv.html

[R69] 生成随机密码
来源：http://hz.sufxvd.cn/gtuqfdgsgn.html

head -c 16 /dev/urandom | base64
来源：http://hz.tanke756.top/gtggvlceix.html

[R70] 时间戳与互转
来源：http://hz.ydjk.org.cn/gtjynitgji.html

date +%s;  date -d @1700000000
来源：http://hz.jinghuilouyu.cn/gtnwtrihng.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtzxmxayda.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtjffbqtat.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gtiumqprtp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.316326.xyz/gtdrvyqnol.html

[R73] 分割大日志
来源：http://hz.jinyuanbaomall.cn/gtmgmdzfpo.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtaijxbrdf.html

[R74] 批量重命名
来源：http://hz.dianchejie.cn/gtfpgkfoqk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guannengcc.top/gtepnbulyz.html

[R75] 导出环境变量
来源：http://hz.chenlongwang.top/gtjdncclam.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sweek.top/gtzqeibgzy.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gtbttowdsm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtuaybkfxa.html

[R77] 读取用户输入
来源：http://hz.dianchejie.cn/gtbxylffdj.html

read -rp "请输入: " ans
来源：http://hz.hnxiangtu.top/gtygkqjmtj.html

[R78] 交互式菜单
来源：http://hz.mhx1999.top/gtgigjaapg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shuidangran.top/gtxpbgyzgh.html

[R79] 解析命令行选项
来源：http://hz.hongshengwenyu.top/gtipqqkgfd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gtuypmpchg.html

[R80] 查看脚本执行耗时
来源：http://hz.yanxiufei.cn/gtkbbahmzz.html

time ./run.sh
来源：http://hz.shzxlz.cn/gtuydyypvz.html

================================================================================
来源：http://hz.hywenlv.cn/gtcohyiicw.html

S. C / C++ 专题
来源：http://hz.jqgufenzy.top/gtzfterusz.html

================================================================================
来源：http://hz.chenzaomai.com/gtmhtpdwde.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtpdflbipb.html

#include <stdio.h>
来源：http://hz.316326.xyz/gtasjriemv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gtkkbxqzta.html

[S02] C：变量与格式化输出
来源：http://hz.jianghu66.top/gttfrkebzw.html

int a = 10; printf("%d\n", a);
来源：http://hz.c1oappe.top/gthvbfzikm.html

[S03] C：读入整数
来源：http://hz.feifeiyinyue.top/gtacpdorye.html

int x; scanf("%d", &x);
来源：http://hz.yanxiufei.cn/gtglqcjdda.html

[S04] C：字符串复制
来源：http://hz.iojbl.cn/gturejvzhb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhoulong.xyz/gtglvhtprl.html

[S05] C：字符串长度
来源：http://hz.hammf.cn/gtsueicrhn.html

strlen(s)
来源：http://hz.0kj1m.cn/gtwviigmjw.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gtckvhxlwz.html

strcmp(a, b) == 0
来源：http://hz.chenlongwang.top/gtwybgloqe.html

[S07] C：数组遍历求和
来源：http://hz.ppjwa.cn/gtthdxwgns.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guannengcc.top/gtrhmtfafz.html

[S08] C：动态内存分配与释放
来源：http://hz.svipenyu.cn/gtxwtexker.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tian-w.cn/gtkehtdgzo.html

[S09] C：结构体定义与初始化
来源：http://hz.andypj.xyz/gtbcjjcmgq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj202588.top/gtgvwoxssw.html

[S10] C：指针与解引用
来源：http://hz.cdnleiting.top/gtxixlghcl.html

int *p = &a;  *p = 5;
来源：http://hz.andypj.xyz/gtrggwiaxs.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtlzgxcczu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtcccnrqcw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtgybwyknt.html

fclose(f);
来源：http://hz.nwbrower.top/gtnvtnwyuw.html

[S12] C：写文件
来源：http://hz.svipenyu.cn/gtfvzpckuv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gogol.net.cn/gtricevtfk.html

[S13] C：宏定义
来源：http://hz.chenjidiqi.icu/gtgeyygfgt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cheryme.top/gtravgpkpz.html

[S14] C：枚举
来源：http://hz.sweek.top/gtyaxdctyd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtyyflhxad.html

[S15] C：类型转换
来源：http://hz.vqdsnc.cn/gtroqanedc.html

(double) a / b
来源：http://hz.ehwqpu.com/gtuipqrxgo.html

[S16] C：位操作置位
来源：http://hz.tanke756.top/gtxsmucrxe.html

x |= (1 << 3);
来源：http://hz.ydjk.org.cn/gtszrjsuox.html

[S17] C：安全拼接字符串
来源：http://hz.havefunace.top/gtibrtlcyi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hongshengwenyu.top/gtkehujujs.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtzjbjvawn.html

int main(int argc, char **argv)
来源：http://hz.smart0.xyz/gtexhhlmoa.html

[S19] C：快速排序
来源：http://hz.yangfankeji.com/gtdsvrjlru.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtkkkdcigv.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtjrmyquyk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.guannengcc.top/gttphvnvse.html

[S21] C：字符类别判断
来源：http://hz.chenzaomai.com/gtefmjxucy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hywenlv.cn/gtcvlgotmy.html

[S22] C：字符串转数字
来源：http://hz.chenzaomai.com/gtuntgdylh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jyoumei.cn/gtruppfkvj.html

[S23] C：随机数
来源：http://hz.sxryk.cn/gtadkjsoae.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtoenrszcl.html

[S24] C：获取本地时间
来源：http://hz.jiagoushi.top/gtkxkpntzj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhijiandao.cn/gtejjmcxzo.html

[S25] C：内存拷贝
来源：http://hz.cashguo.top/gtwnffsyyw.html

memcpy(dst, src, n);
来源：http://hz.sysykeji.top/gtzvulxzhy.html

[S26] C：内存清零
来源：http://hz.snrcjt.cn/gthpurzqph.html

memset(a, 0, sizeof a);
来源：http://hz.redwolf501.top/gtobpiwyyy.html

[S27] C：定义常量
来源：http://hz.havefunace.top/gtjsvgtbcp.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtzgdoyctj.html

[S28] C：静态变量
来源：http://hz.jinqigufen.top/gtjodhrypv.html

static int counter = 0;
来源：http://hz.yongpay.top/gtugkypvyq.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtcbofsufv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hywenlv.cn/gtbluwnjaf.html

[S30] C：头文件保护
来源：http://hz.c1oappe.top/gtbbyjflvn.html

#ifndef X_H
来源：http://hz.xuanzx.com/gtytbmvsmz.html

#define X_H
来源：http://hz.jinqigufen.top/gtkfphrkre.html

#endif
来源：http://hz.gzhubu.top/gttwjqiacy.html

[S31] C++：Hello World
来源：http://hz.yj202588.top/gtrlbxzvjh.html

#include <iostream>
来源：http://hz.hongshengwenyu.top/gtakrkksdl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hammf.cn/gtvxmhkips.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gtaqinssqq.html

std::string s = "hi";  s += "!";
来源：http://hz.jqgfzy.top/gtxdqmvmqi.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangtech.top/gtfouyabsw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxinkj.top/gtkijkoyjh.html

[S34] C++：遍历 vector
来源：http://hz.xylfe.cn/gtuuhsfjcq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ppjwa.cn/gtzkbaifez.html

[S35] C++：map
来源：http://hz.hfpthk.cn/gtsqjvpgxf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtwhfydypg.html

[S36] C++：unordered_map
来源：http://hz.chenjidiqi.icu/gtudmowcgx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtrkdmabja.html

[S37] C++：set
来源：http://hz.tianlin.xyz/gtiunptzng.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jlsjyb.cn/gtnwyqffpt.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtunketuge.html

std::sort(v.begin(), v.end());
来源：http://hz.jyoumei.cn/gtdplrsxdf.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtrcjlgwed.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daria6918.cn/gtrjnyfpqi.html

[S40] C++：查找元素
来源：http://hz.chenjidiqi.icu/gtqdvvizpv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtjpqwlbmp.html

[S41] C++：类与构造函数
来源：http://hz.ehwqpu.com/gtpzqfgnwi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtnnanpntx.html

[S42] C++：继承与虚函数
来源：http://hz.quarkkingdee.top/gtttdkhhvp.html

class B : public Base { public: void f() override {} };
来源：http://hz.pycfn.com/gtdkevccct.html

[S43] C++：智能指针
来源：http://hz.yj20258888.top/gttejvugma.html

auto p = std::make_unique<int>(5);
来源：http://hz.svipenyu.cn/gtwpmgvijv.html

[S44] C++：引用传参
来源：http://hz.shzxlz.cn/gtlvroqcgg.html

void inc(int &x) { ++x; }
来源：http://hz.tanke756.top/gtkydmmqtb.html

[S45] C++：lambda
来源：http://hz.xylfe.cn/gtwuqbzfjl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xinyue.icu/gthlfrzgvz.html

[S46] C++：函数模板
来源：http://hz.yvedp.cn/gtskqkcrdd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hywenlv.cn/gtfyoujgjs.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtswaidbih.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhaomingkeji.xyz/gtvupezklp.html

[S48] C++：逐行读文件
来源：http://hz.zhijiandao.cn/gtlqwockxt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtyxcmdjrx.html

while (std::getline(in, line)) { }
来源：http://hz.ydzc1.top/gthabljvsb.html

[S49] C++：写文件
来源：http://hz.xuetiantiany.cn/gtxymutroz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xylfe.cn/gtcskhfboj.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtvdcainnu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ehwqpu.com/gtdrqzpfgj.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gtzxickndj.html

static_cast<double>(a) / b
来源：http://hz.gaohongyu789.top/gtoonoehxe.html

[S52] C++：const 与 noexcept
来源：http://hz.cheryme.top/gtyiebtigm.html

int size() const noexcept { return n_; }
来源：http://hz.andypj.xyz/gtpekhyqqf.html

[S53] C++：移动语义
来源：http://hz.iojbl.cn/gtaihhxfqt.html

std::vector<int> w = std::move(v);
来源：http://hz.yuxming.cn/gtwvdwgrlr.html

[S54] C++：异常处理
来源：http://hz.ydzc1.top/gtgvmiztbn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.svipenyu.cn/gtazvqlgdw.html

[S55] C++：结构化绑定
来源：http://hz.pengpengdd.cyou/gtrkawpxdd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pycfn.com/gtuzucwzor.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtwtwrrakj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nwbrower.top/gtsddjjaaz.html

[S57] C++：编译期常量
来源：http://hz.jinyuanbaomall.cn/gtrafmsbkd.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gtmrrssdhk.html

[S58] C++：命名空间
来源：http://hz.mhx1999.top/gtowgjlvhs.html

namespace ns { int f() { return 1; } }
来源：http://hz.sweek.top/gtqsgxcppo.html

[S59] C++：静态断言
来源：http://hz.pengpengdd.cyou/gtyyejwvml.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhixingplan.top/gtbijprbyn.html

[S60] C++：遍历并删除元素
来源：http://hz.wangdashe.top/gthbgwybwu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cucudq.cn/gteweacijl.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtazjxxrwu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhengqikj.top/gtabtzxdpq.html

================================================================================
来源：http://hz.ydjk.org.cn/gtiwhfbjdv.html

[T01] Kotlin：Hello World
来源：http://hz.jqgufenzy.top/gtfddgsmgd.html

println("Hello")
来源：http://hz.birdmap.top/gtmyinropv.html

[T02] Kotlin：变量
来源：http://hz.cdnleiting.top/gtmjuqzlyf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.0kj1m.cn/gtggcimvet.html

[T03] Kotlin：字符串模板
来源：http://hz.guowangkeji.top/gthxlnbcoj.html

"值: $b"
来源：http://hz.jqgfzy.top/gtzgwizfdp.html

[T04] Kotlin：空安全
来源：http://hz.cdnleiting.top/gttcukjtem.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtypufvbpa.html

[T05] Kotlin：when 表达式
来源：http://hz.yuanzhike.top/gtyjpejofn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.bjfxy.top/gtkorylvvy.html

[T06] Kotlin：集合映射
来源：http://hz.hysaishi.cn/gtuhhipzuy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtlqtigngv.html

[T07] Kotlin：集合过滤
来源：http://hz.yvedp.cn/gtsktptfzt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.svipenyu.cn/gtpcrqmyfs.html

[T08] Kotlin：数据类
来源：http://hz.svipenyu.cn/gtgbchrsfs.html

data class User(val name: String, val age: Int)
来源：http://hz.wangdashe.top/gthultjmcd.html

[T09] Kotlin：扩展函数
来源：http://hz.zycfv.cn/gtoigzftho.html

fun String.exclaim() = this + "!"
来源：http://hz.bjfxy.top/gtnavkgqid.html

[T10] Kotlin：默认参数
来源：http://hz.jinghuilouyu.cn/gtcbcdzlch.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yueranfly.top/gtsmvqpbie.html

[T11] Kotlin：协程
来源：http://hz.jqgufenzy.top/gtlepueqcv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.kuanghao11.cn/gtfkaorfcv.html

[T12] Kotlin：解构声明
来源：http://hz.sweek.top/gtzbprctxv.html

val (a, b) = Pair(1, 2)
来源：http://hz.aizwys.cn/gtcdxphsnz.html

[T13] Kotlin：只读 Map
来源：http://hz.svipenyu.cn/gtbpwhttos.html

val m = mapOf("a" to 1)
来源：http://hz.haohaochexian.top/gtgrnhyxnm.html

[T14] Kotlin：循环
来源：http://hz.dashuyun.cn/gtzwdhoxng.html

for (i in 1..10) println(i)
来源：http://hz.gaohongyu789.top/gtthmrfhhx.html

[T15] Kotlin：接口
来源：http://hz.feifeiyinyue.top/gtohmralnu.html

interface Shape { fun area(): Double }
来源：http://hz.ppjwa.cn/gtoddhedaf.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gtvxbfksrg.html

print("Hello")
来源：http://hz.gzhubu.top/gteujiabpd.html

[T17] Swift：变量与常量
来源：http://hz.nwbrower.top/gtaqfyaonf.html

var a = 1;  let b = 2
来源：http://hz.kuanghao11.cn/gtiwnfgnxb.html

[T18] Swift：字符串插值
来源：http://hz.havefunace.top/gtzigngpjy.html

"值: \(b)"
来源：http://hz.hnqzz.top/gtgsimzthv.html

[T19] Swift：可选绑定
来源：http://hz.xziqi.cn/gtbuwcsykx.html

if let n = opt { print(n) }
来源：http://hz.haohaochexian.top/gtwaobsysb.html

[T20] Swift：数组操作
来源：http://hz.gaohongyu789.top/gtllderyfl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigfzy.top/gtwpkvmnyr.html

[T21] Swift：遍历
来源：http://hz.yuxming.cn/gtqtlschfz.html

for x in a { print(x) }
来源：http://hz.xuetiantiany.cn/gtnjfoczlp.html

[T22] Swift：字典
来源：http://hz.yvedp.cn/gttbzftqnn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xuanzx.com/gtwhbaulyz.html

[T23] Swift：函数
来源：http://hz.zhengqikj.top/gtrolnuvps.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gogol.net.cn/gtkebnjckh.html

[T24] Swift：闭包
来源：http://hz.jianghu66.top/gtzofbvvfn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.vqdsnc.cn/gtdryidkij.html

[T25] Swift：结构体
来源：http://hz.andypj.xyz/gtapqyhgcx.html

struct P { var x: Int }
来源：http://hz.sysykeji.top/gtmxadhzsx.html

[T26] Swift：类与重写
来源：http://hz.yongpay.top/gtirqomjve.html

class A: Base { override func f() {} }
来源：http://hz.aibaodan.cn/gtbdwxzzjz.html


<!-- 参考信息 -->