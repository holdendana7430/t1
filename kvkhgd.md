代发 wailian999

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gtyasyvzek.html

[R20] 关联数组（字典）
来源：http://hz.gaohongyu789.top/gthevzhgfr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtqfkvsepm.html

[R21] 字符串长度
来源：http://hz.sxryk.cn/gtkvdirrvc.html

echo "${#s}"
来源：http://hz.hnxiangtu.top/gtdhorqiit.html

[R22] 截取子串
来源：http://hz.birdmap.top/gtbdyoelra.html

echo "${s:0:5}"
来源：http://hz.chenjidiqi.icu/gtzrxzdfwe.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtmbfwrrtp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhaomingkeji.xyz/gtwncsrcfn.html

[R24] 大小写转换
来源：http://hz.ydjk.org.cn/gteyivevnp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhengqikj.top/gtzxjddalx.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenjidiqi.icu/gtkqadcqcg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nanxinkj.top/gtnqrfhibt.html

[R26] 命令替换
来源：http://hz.ppjwa.cn/gtomhedfpp.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtuacqpmja.html

[R27] 算术展开
来源：http://hz.jqgufenzy.top/gtqcbpbbxm.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtbvadnywy.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtngeykuji.html

echo "scale=2; 10/3" | bc
来源：http://hz.hysaishi.cn/gtunatyvin.html

[R29] 定义函数
来源：http://hz.jqgufenzy.top/gtabzqdcrv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gotoacloud.top/gtqzuuajzt.html

[R30] 函数返回状态码
来源：http://hz.gogol.net.cn/gtawrysivv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtdutljtyw.html

[R31] 局部变量
来源：http://hz.shanyushiyangkeji.top/gtckyliprp.html

f() { local x=1; echo "$x"; }
来源：http://hz.pycfn.com/gtsujhtwle.html

[R32] 参数个数校验
来源：http://hz.quarkkingdee.top/gtomsxqiqq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuxming.cn/gtalpqipyn.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gttczihxyv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gtxlmwbbyx.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gtqlpnjqrv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.fengsongda.top/gtyqeqkqut.html

[R35] 后台执行并等待
来源：http://hz.yuxming.cn/gtfdxniohd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tanke756.top/gtzlmoupkg.html

[R36] 并发执行多个任务
来源：http://hz.nanxuanxn.top/gtuwfebapx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gtogprtykm.html

[R37] 把输出赋给变量
来源：http://hz.sxryk.cn/gtinwvplbc.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtodgttyjt.html

[R38] 管道串联
来源：http://hz.yongpay.top/gtvknvjfdf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtvzkrcgai.html

[R39] 重定向标准输出与错误
来源：http://hz.jianghu66.top/gtctywbsua.html

cmd > out.log 2>&1
来源：http://hz.tanke756.top/gtatzioccb.html

[R40] 追加写日志
来源：http://hz.jyoumei.cn/gtotympfoa.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gttwzbmhdo.html

[R41] 丢弃输出
来源：http://hz.hywenlv.cn/gtbargfpop.html

cmd >/dev/null 2>&1
来源：http://hz.daxiang520.top/gtxsnhbwdb.html

[R42] 输入重定向
来源：http://hz.svipenyu.cn/gtujftnxzq.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtnhnoofjv.html

[R43] 按名字查找文件
来源：http://hz.smart0.xyz/gtbuetkakl.html

find . -name "*.log" -type f
来源：http://hz.gotoacloud.top/gtltmtguns.html

[R44] 按修改时间查找
来源：http://hz.jinyuanbaomall.cn/gttkhkbbhm.html

find . -mtime -7 -type f
来源：http://hz.hnxiangtu.top/gtdjdceepu.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtcwimcfkh.html

find . -name "*.tmp" -delete
来源：http://hz.kuanghao11.cn/gtpatlmglv.html

[R46] 递归替换文件内容
来源：http://hz.zhijiandao.cn/gtvzvksxap.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hongshengwenyu.top/gtjrfybmmn.html

[R47] sed 单行替换
来源：http://hz.gogol.net.cn/gtgogbeyza.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.mhx1999.top/gtjuadzaia.html

[R48] awk 取指定列
来源：http://hz.ybcxt.top/gtomjompgy.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtexshkgug.html

[R49] awk 带条件
来源：http://hz.jqgfzy.top/gtcmrkreek.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtnklaxjbb.html

[R50] awk 求和
来源：http://hz.zdqjudy.top/gtqaleliii.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ivvv.top/gtejptwtld.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gtfzuidain.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gthpmgbmvk.html

[R52] 统计行数
来源：http://hz.pengpengdd.cyou/gtvqbywcfl.html

wc -l a.txt
来源：http://hz.smart0.xyz/gtrydqmibj.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtqrcjsudx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aizwys.cn/gtuwbwbpfu.html

[R54] 比较两个文件
来源：http://hz.ppjwa.cn/gtcljtvyxh.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtquvqdifj.html

[R55] 压缩与解压
来源：http://hz.nanxinkj.top/gtcljfgvuf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.fengsongda.top/gteseojvvw.html

[R56] 远程拷贝
来源：http://hz.snrcjt.cn/gtnnwxnixr.html

scp file user@host:/path/
来源：http://hz.haohaochexian.top/gtrnfkmmeg.html

[R57] 远程执行命令
来源：http://hz.aibaodan.cn/gtfqzhcsli.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gtbjefvrca.html

[R58] 下载文件
来源：http://hz.tian-w.cn/gtmgzkcbjt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guowangkeji.top/gtbzqhrwjt.html

[R59] 发 POST JSON
来源：http://hz.tian-w.cn/gtuavwbhqb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daxiang520.top/gtludizxif.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj202588.top/gtwmuaaoyk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.haohaochexian.top/gtyvymrtcx.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtcvizaywm.html

df -h;  du -sh *
来源：http://hz.jiagoushi.top/gteijfjbrc.html

[R62] 找最占空间的文件
来源：http://hz.yvedp.cn/gtrggakdja.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtgfivznyh.html

[R63] 内存与进程
来源：http://hz.wangdashe.top/gtakosgncc.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258888.top/gtwcqjpujr.html

[R64] 结束进程
来源：http://hz.jqgfzy.top/gtnxgtzutq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.dashuyun.cn/gtizmrxxgk.html

[R65] 查看端口占用
来源：http://hz.redwolf501.top/gthfdvhgyf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nanxuanxn.top/gtadxgdtvg.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gteyepnajp.html

crontab -e;  crontab -l
来源：http://hz.jinqigufen.top/gtwshvyjun.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gthipujfhe.html

openssl rand -hex 16
来源：http://hz.jinghuilouyu.cn/gtaxiagxuo.html

[R68] 计算文件校验值
来源：http://hz.zhijiandao.cn/gtablhbtfs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydjk.org.cn/gtqezcayax.html

[R69] 生成随机密码
来源：http://hz.yanxiufei.cn/gthwoxbjzc.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258.top/gtgormqbcy.html

[R70] 时间戳与互转
来源：http://hz.dianchejie.cn/gtenchvkwu.html

date +%s;  date -d @1700000000
来源：http://hz.hywenlv.cn/gtrdeekjmi.html

[R71] 日期格式化
来源：http://hz.guannengcc.top/gtgmtxcfnx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangkeji.top/gtuxlvjcoj.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gtwbjydoox.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cdnleiting.top/gtqphdbjrk.html

[R73] 分割大日志
来源：http://hz.cdnleiting.top/gtmxjmvzmr.html

split -l 1000 big.log part_
来源：http://hz.gaohongyu789.top/gthvsnjbac.html

[R74] 批量重命名
来源：http://hz.zycfv.cn/gtfozvcuak.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guowangkeji.top/gtiyufidrv.html

[R75] 导出环境变量
来源：http://hz.jinqigufen.top/gtzzoybomd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gtmfgkhqjn.html

[R76] 使用临时文件
来源：http://hz.jinghuilouyu.cn/gtuxidbmkm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtnugguroj.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtrrslttpx.html

read -rp "请输入: " ans
来源：http://hz.yvedp.cn/gtbxeosydz.html

[R78] 交互式菜单
来源：http://hz.feifeiyinyue.top/gtbvzvcrsl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.0kj1m.cn/gtkxczgjkh.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtzrotqdnv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hnqzz.top/gtvocpjguw.html

[R80] 查看脚本执行耗时
来源：http://hz.chenjidiqi.icu/gtwbhvieti.html

time ./run.sh
来源：http://hz.guannengcc.top/gtyjaxtvfr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtttgdftde.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gttharenwm.html

================================================================================
来源：http://hz.yonumen.top/gtqmjidbpi.html

[S01] C：Hello World
来源：http://hz.jqgfzy.top/gtdivdqiyf.html

#include <stdio.h>
来源：http://hz.bjfxy.top/gtnltoupsc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtralahulo.html

[S02] C：变量与格式化输出
来源：http://hz.c1oappe.top/gtkvelxika.html

int a = 10; printf("%d\n", a);
来源：http://hz.guowangkeji.top/gtdsqwntcp.html

[S03] C：读入整数
来源：http://hz.zhoulong.xyz/gtzpummoes.html

int x; scanf("%d", &x);
来源：http://hz.shuidangran.top/gtbtxjobjn.html

[S04] C：字符串复制
来源：http://hz.havefunace.top/gtbseawrak.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nwbrower.top/gtzfqsmkuy.html

[S05] C：字符串长度
来源：http://hz.hywenlv.cn/gtcoxayyrx.html

strlen(s)
来源：http://hz.gaohongyu789.top/gtiytpxgbs.html

[S06] C：字符串比较
来源：http://hz.yj20258.top/gtcbvgunsp.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtuxoqebhy.html

[S07] C：数组遍历求和
来源：http://hz.cqqwz.cn/gtpxnzppsu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangtech.top/gtsilskoxy.html

[S08] C：动态内存分配与释放
来源：http://hz.chenlongwang.top/gtvovcmkne.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sufxvd.cn/gtoelxgybj.html

[S09] C：结构体定义与初始化
来源：http://hz.cqqwz.cn/gtpjjwjpzw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fengsongda.top/gtanuqlbra.html

[S10] C：指针与解引用
来源：http://hz.aizwys.cn/gtunmkhxtm.html

int *p = &a;  *p = 5;
来源：http://hz.zhongyouzk.top/gtdbinofni.html

[S11] C：逐行读文件
来源：http://hz.jinqigfzy.top/gtzexgxunf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhengqikj.top/gtstreahcb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangdashe.top/gtqftkfslz.html

fclose(f);
来源：http://hz.zhengqikj.top/gtykrrfesx.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtfyyujqng.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gtehkrjbri.html

[S13] C：宏定义
来源：http://hz.yj20258888.top/gtkijkpkbf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtriqgbbbx.html

[S14] C：枚举
来源：http://hz.nanxuanxn.top/gtucijvgxp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gtnmjmowqg.html

[S15] C：类型转换
来源：http://hz.shanyushiyangtech.top/gtdmalzysd.html

(double) a / b
来源：http://hz.zhongyouzk.top/gtmhxckkrw.html

[S16] C：位操作置位
来源：http://hz.yanxiufei.cn/gtlkjhalfj.html

x |= (1 << 3);
来源：http://hz.ivvv.top/gtmkcwcbrb.html

[S17] C：安全拼接字符串
来源：http://hz.gotoacloud.top/gtzqquqsqe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xziqi.cn/gtxvszuepj.html

[S18] C：命令行参数
来源：http://hz.yueranfly.top/gtmxlewshs.html

int main(int argc, char **argv)
来源：http://hz.cheryme.top/gtkupajjrj.html

[S19] C：快速排序
来源：http://hz.pengpengdd.cyou/gtzcawfthw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtpgddpwai.html

[S20] C：二分查找
来源：http://hz.yj202588.top/gtgpvucuws.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtpwmgssvv.html

[S21] C：字符类别判断
来源：http://hz.ywan-chungtsiang.top/gtnpegmoif.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigfzy.top/gtvtwfbhtk.html

[S22] C：字符串转数字
来源：http://hz.52xcode.cn/gtvbudmdly.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtfseqcyhi.html

[S23] C：随机数
来源：http://hz.shangyingyoupin.top/gtwpvihyvk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xinyue.icu/gtraglukxc.html

[S24] C：获取本地时间
来源：http://hz.0kj1m.cn/gtbcrnlxbn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hywenlv.cn/gtyfituaak.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtberhciij.html

memcpy(dst, src, n);
来源：http://hz.jianghu66.top/gtzywlplpu.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gtxdltjxcx.html

memset(a, 0, sizeof a);
来源：http://hz.xuanzx.com/gtzemesqqi.html

[S27] C：定义常量
来源：http://hz.9152youxi.cn/gtwfxkqfwt.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtefzpaohw.html

[S28] C：静态变量
来源：http://hz.birdmap.top/gtznvrcuck.html

static int counter = 0;
来源：http://hz.fengsongda.top/gtvybnxrqc.html

[S29] C：变参函数
来源：http://hz.nanxinkj.top/gturjdzcom.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtogypelad.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gtvrofmksx.html

#ifndef X_H
来源：http://hz.zhoulong.xyz/gtwxwbytay.html

#define X_H
来源：http://hz.daxiang520.top/gthdmdkizj.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gtxnshruah.html

[S31] C++：Hello World
来源：http://hz.haohaochexian.top/gtfqzpxnpm.html

#include <iostream>
来源：http://hz.dashuyun.cn/gtpwrgcltj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cqqwz.cn/gtkgbwhfzd.html

[S32] C++：字符串
来源：http://hz.haohaochexian.top/gtlgrnkmns.html

std::string s = "hi";  s += "!";
来源：http://hz.xziqi.cn/gtgesucovz.html

[S33] C++：vector 增删
来源：http://hz.shangyingyoupin.top/gtelcwesop.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtivhgsyuv.html

[S34] C++：遍历 vector
来源：http://hz.jqgufenzy.top/gtlfuuterb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtkwqorpca.html

[S35] C++：map
来源：http://hz.jinyuanbaomall.cn/gtwldvedgk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtfdozfump.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gtwszfhltd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtsfpgkoub.html

[S37] C++：set
来源：http://hz.fengsongda.top/gtkrazadtk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.smart0.xyz/gtlbioohsm.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtcbxphpvr.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtbhfvlpjq.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gttcdiqkwj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhaomingkeji.xyz/gtgsspgvec.html

[S40] C++：查找元素
来源：http://hz.c1oappe.top/gtxhtcyqkw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fengsongda.top/gtmzxkemwp.html

[S41] C++：类与构造函数
来源：http://hz.yuxming.cn/gtdhhenxxv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tanke756.top/gttoxkcraw.html

[S42] C++：继承与虚函数
来源：http://hz.cdnleiting.top/gtbtfeummz.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhiwuduotai.top/gtjjvjhobt.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gtwonaebum.html

auto p = std::make_unique<int>(5);
来源：http://hz.haohaochexian.top/gtcbkymnqf.html

[S44] C++：引用传参
来源：http://hz.shuidangran.top/gtbqctsawm.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gtcvqraaca.html

[S45] C++：lambda
来源：http://hz.xingfuxueyuan.xyz/gtqkizscoe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtexnklehx.html

[S46] C++：函数模板
来源：http://hz.316326.xyz/gtlhmmxrpl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgufenzy.top/gtasfaghzj.html

[S47] C++：结构化绑定遍历
来源：http://hz.xylfe.cn/gtmubsuzkq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zycfv.cn/gtpbxaqgai.html

[S48] C++：逐行读文件
来源：http://hz.ppjwa.cn/gtxvhjhsso.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gtdkszgtfr.html

while (std::getline(in, line)) { }
来源：http://hz.guowangkeji.top/gtibsnosqr.html

[S49] C++：写文件
来源：http://hz.gogol.net.cn/gtrsjaxkgt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.haohaochexian.top/gtncixephs.html

[S50] C++：格式化数字
来源：http://hz.andypj.xyz/gtfvjrwipw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangdashe.top/gtutmvxbsb.html

[S51] C++：显式类型转换
来源：http://hz.zhoulong.xyz/gtfhdnkoaw.html

static_cast<double>(a) / b
来源：http://hz.jiagoushi.top/gtsieihumt.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgufenzy.top/gtsqoyalrf.html

int size() const noexcept { return n_; }
来源：http://hz.daxiang520.top/gtugevodtn.html

[S53] C++：移动语义
来源：http://hz.hywenlv.cn/gtelbmzpmt.html

std::vector<int> w = std::move(v);
来源：http://hz.kuanghao11.cn/gtcsuqwoit.html

[S54] C++：异常处理
来源：http://hz.c1oappe.top/gtjuvpjxmk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hammf.cn/gtwggsxdgl.html

[S55] C++：结构化绑定
来源：http://hz.ybcxt.top/gtybwnvmfr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ywan-chungtsiang.top/gtxsiwzvpq.html

[S56] C++：optional
来源：http://hz.yongpay.top/gtwujwvwjr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tian-w.cn/gtdgpdglto.html

[S57] C++：编译期常量
来源：http://hz.wangshuangyany.cn/gtkbxzvnmz.html

constexpr int N = 10;
来源：http://hz.zhaomingkeji.xyz/gtyjeiffaw.html

[S58] C++：命名空间
来源：http://hz.gzhubu.top/gtwroakqyx.html

namespace ns { int f() { return 1; } }
来源：http://hz.yangfankeji.com/gtetpjwigq.html

[S59] C++：静态断言
来源：http://hz.cdnleiting.top/gtepyeweie.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuanzhike.top/gtwmejfnvc.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxinkj.top/gtzudkdnsg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cashguo.top/gtuogbgxib.html

================================================================================
来源：http://hz.52xcode.cn/gtiubvkaxl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtiiapupsq.html

================================================================================
来源：http://hz.jiagoushi.top/gtfskutqmr.html

[T01] Kotlin：Hello World
来源：http://hz.zdqjudy.top/gtqarhvyvd.html

println("Hello")
来源：http://hz.hfpthk.cn/gtsamnmqis.html

[T02] Kotlin：变量
来源：http://hz.52xcode.cn/gtwthgmphi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jlsjyb.cn/gtxpomwjrh.html

[T03] Kotlin：字符串模板
来源：http://hz.sweek.top/gtoiddiimd.html

"值: $b"
来源：http://hz.yongpay.top/gtojumxitf.html

[T04] Kotlin：空安全
来源：http://hz.zhixingplan.top/gtwknddtvb.html

val n: String? = null;  n?.length
来源：http://hz.hnqzz.top/gtfrvycacy.html

[T05] Kotlin：when 表达式
来源：http://hz.gotoacloud.top/gtvlovuesz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ywan-chungtsiang.top/gtvutimoyi.html

[T06] Kotlin：集合映射
来源：http://hz.cqqwz.cn/gttlsovuhl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ybcxt.top/gthjzpwipi.html

[T07] Kotlin：集合过滤
来源：http://hz.ydjk.org.cn/gtcbeaofho.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhongyouzk.top/gtfgzzgrxd.html

[T08] Kotlin：数据类
来源：http://hz.tianlin.xyz/gtxnotjtps.html

data class User(val name: String, val age: Int)
来源：http://hz.jyoumei.cn/gtakejqkyo.html

[T09] Kotlin：扩展函数
来源：http://hz.0kj1m.cn/gtywepdjjg.html

fun String.exclaim() = this + "!"
来源：http://hz.yongpay.top/gtnpmnfpjz.html

[T10] Kotlin：默认参数
来源：http://hz.zhixingplan.top/gtjqgfxtya.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jlsjyb.cn/gtmgapqcwq.html

[T11] Kotlin：协程
来源：http://hz.yangfankeji.com/gtzpyepprc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jlsjyb.cn/gtcrghfamz.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtmfqyerqg.html

val (a, b) = Pair(1, 2)
来源：http://hz.havefunace.top/gtbcygkzqv.html

[T13] Kotlin：只读 Map
来源：http://hz.zhengqikj.top/gtqjexrrub.html

val m = mapOf("a" to 1)
来源：http://hz.ppjwa.cn/gtnluvhspu.html

[T14] Kotlin：循环
来源：http://hz.guowangkeji.top/gtzcyldllw.html

for (i in 1..10) println(i)
来源：http://hz.ivvv.top/gtfnqllxmn.html

[T15] Kotlin：接口
来源：http://hz.cdnleiting.top/gtudwdoins.html

interface Shape { fun area(): Double }
来源：http://hz.jinyuanbaomall.cn/gtsfqyeslf.html

[T16] Swift：Hello World
来源：http://hz.jinqigufen.top/gttedywutz.html

print("Hello")
来源：http://hz.9152youxi.cn/gtwkophrla.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangtech.top/gtwiigscey.html

var a = 1;  let b = 2
来源：http://hz.zhengqikj.top/gtlylidmso.html

[T18] Swift：字符串插值
来源：http://hz.zhijiandao.cn/gtyjyyzfdq.html

"值: \(b)"
来源：http://hz.shanyushiyangtech.top/gtwdrdjltv.html

[T19] Swift：可选绑定
来源：http://hz.yj20258.top/gthgsipalk.html

if let n = opt { print(n) }
来源：http://hz.ivvv.top/gtedcpztxv.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gthxyoubiy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigfzy.top/gttqleblvm.html

[T21] Swift：遍历
来源：http://hz.tianlin.xyz/gtuyfwqouq.html

for x in a { print(x) }
来源：http://hz.tian-w.cn/gtesaxcbye.html

[T22] Swift：字典
来源：http://hz.zycfv.cn/gthumvtcpv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sxryk.cn/gtmetdjdhm.html


<!-- 参考信息 -->