代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhaomingkeji.xyz/gtktbhumyy.html

[R18] 遍历数组
来源：http://hz.yongpay.top/gtsmbwjjqo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ywan-chungtsiang.top/gtezdpulwe.html

[R19] 数组长度
来源：http://hz.zhengqikj.top/gtpaxvhnnm.html

echo "${#arr[@]}"
来源：http://hz.sufxvd.cn/gtuymsnzsz.html

[R20] 关联数组（字典）
来源：http://hz.havefunace.top/gtybqiccuw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.9152youxi.cn/gtdeklwjvf.html

[R21] 字符串长度
来源：http://hz.redwolf501.top/gtbjwpikot.html

echo "${#s}"
来源：http://hz.yj20258.top/gtqkdpronq.html

[R22] 截取子串
来源：http://hz.xingfuxueyuan.xyz/gtznyqpfwb.html

echo "${s:0:5}"
来源：http://hz.shanyushiyangtech.top/gthkrwjzeu.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtplexdysf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guowangkeji.top/gtjwyjcvjg.html

[R24] 大小写转换
来源：http://hz.cqqwz.cn/gtvcpommdy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yangfankeji.com/gtdxkborxw.html

[R25] 去后缀 / 去前缀
来源：http://hz.cdnleiting.top/gtfrnhbkdd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.mhx1999.top/gtdhbpmfxc.html

[R26] 命令替换
来源：http://hz.gzhubu.top/gtobhpweqb.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxuanxn.top/gtuezprlab.html

[R27] 算术展开
来源：http://hz.yj202588.top/gtlsonqigc.html

echo $((1 + 2 * 3))
来源：http://hz.bjfxy.top/gtjlzacivp.html

[R28] 浮点运算
来源：http://hz.zhengqikj.top/gtcroanpth.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhoulong.xyz/gtfnlyvgax.html

[R29] 定义函数
来源：http://hz.zhijiandao.cn/gtpazuioyt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shuidangran.top/gtwhzvqeds.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtkkzmsgwa.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tanke756.top/gtjqzutkhv.html

[R31] 局部变量
来源：http://hz.xylfe.cn/gtatcpugpu.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigufen.top/gtlvbdzzqg.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gtslfwnpkw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtyiutoagx.html

[R33] 捕获错误并提示行号
来源：http://hz.xinyue.icu/gtqulxhtjr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yanxiufei.cn/gtdgnepwnw.html

[R34] 退出时清理
来源：http://hz.tian-w.cn/gtrhwmxvny.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtymnwcalp.html

[R35] 后台执行并等待
来源：http://hz.zhongyouzk.top/gtbioauzac.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydjk.org.cn/gtyrnulhip.html

[R36] 并发执行多个任务
来源：http://hz.gogol.net.cn/gtcfuwstaj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtsqpmoooi.html

[R37] 把输出赋给变量
来源：http://hz.havefunace.top/gtyljmwbxh.html

files=$(ls -1)
来源：http://hz.9152youxi.cn/gtfdgmogfj.html

[R38] 管道串联
来源：http://hz.yonumen.top/gtjzkrfmet.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pengpengdd.cyou/gtqlpfbiwu.html

[R39] 重定向标准输出与错误
来源：http://hz.wangdashe.top/gtsknqxoyj.html

cmd > out.log 2>&1
来源：http://hz.mhx1999.top/gtpjtpydlm.html

[R40] 追加写日志
来源：http://hz.sysykeji.top/gtmnowylym.html

echo "log" >> out.log
来源：http://hz.xziqi.cn/gtnygbgcbn.html

[R41] 丢弃输出
来源：http://hz.jinqigfzy.top/gtxgapbrca.html

cmd >/dev/null 2>&1
来源：http://hz.hnqzz.top/gthoyzpfsd.html

[R42] 输入重定向
来源：http://hz.zdqjudy.top/gtgzrpzxue.html

wc -l < a.txt
来源：http://hz.vqdsnc.cn/gttnttmolr.html

[R43] 按名字查找文件
来源：http://hz.sweek.top/gtoewbiatk.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gtltzkblcn.html

[R44] 按修改时间查找
来源：http://hz.jinqigfzy.top/gtuelxpkpb.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtjeaddhfo.html

[R45] 批量删除
来源：http://hz.c1oappe.top/gtvmiysgsg.html

find . -name "*.tmp" -delete
来源：http://hz.ivvv.top/gtfbmauzim.html

[R46] 递归替换文件内容
来源：http://hz.tianlin.xyz/gtnazqkefr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sysykeji.top/gtxzrtesfa.html

[R47] sed 单行替换
来源：http://hz.mhx1999.top/gtjxuwxjbm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.svipenyu.cn/gttgukbdrz.html

[R48] awk 取指定列
来源：http://hz.jinyuanbaomall.cn/gtorevxudj.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtfbzwhcqp.html

[R49] awk 带条件
来源：http://hz.jinyuanbaomall.cn/gtkzpylvdt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gogol.net.cn/gtjaqzofgo.html

[R50] awk 求和
来源：http://hz.feifeiyinyue.top/gtewpqbezk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tanke756.top/gtnddpjjzi.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gttiynmqek.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinqigufen.top/gtqsfyexcq.html

[R52] 统计行数
来源：http://hz.jianghu66.top/gtfmaerdkq.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtatqptdvu.html

[R53] 查看文件头与实时尾
来源：http://hz.zycfv.cn/gtayqwdnpv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtxrusxnle.html

[R54] 比较两个文件
来源：http://hz.shangyingyoupin.top/gtwjhaytgr.html

diff a.txt b.txt
来源：http://hz.meibo888.top/gtfpkaznzk.html

[R55] 压缩与解压
来源：http://hz.tianlin.xyz/gtlffvcqtt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shangyingyoupin.top/gtvifknpsu.html

[R56] 远程拷贝
来源：http://hz.zhijiandao.cn/gtojhkmlqi.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gtscjwoggp.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtlhardbfv.html

ssh user@host 'uptime'
来源：http://hz.pycfn.com/gtjgcmhuon.html

[R58] 下载文件
来源：http://hz.havefunace.top/gtupfikcbt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenjidiqi.icu/gtupzglrss.html

[R59] 发 POST JSON
来源：http://hz.pycfn.com/gtnuyoaqtx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nwbrower.top/gtzspdhnkw.html

[R60] 只看 HTTP 状态码
来源：http://hz.jiagoushi.top/gtgcovuwcw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.meibo888.top/gtfkduhrtr.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtxzfpvltl.html

df -h;  du -sh *
来源：http://hz.yj20258.top/gtadzvvwqc.html

[R62] 找最占空间的文件
来源：http://hz.hnqzz.top/gttbgwcpek.html

du -ah . | sort -rh | head -10
来源：http://hz.cucudq.cn/gtcqsmeecl.html

[R63] 内存与进程
来源：http://hz.chenjidiqi.icu/gtaxkteahc.html

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtuboulfkp.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gtqceqkphz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtduuermxu.html

[R65] 查看端口占用
来源：http://hz.chenjidiqi.icu/gtieilfiad.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gtdmxzuzgg.html

[R66] 定时任务
来源：http://hz.zhongyouzk.top/gtkgpgaviq.html

crontab -e;  crontab -l
来源：http://hz.gotoacloud.top/gtoknocbdu.html

[R67] 生成随机十六进制串
来源：http://hz.cheryme.top/gtvpfaisco.html

openssl rand -hex 16
来源：http://hz.cucudq.cn/gtzdmizqft.html

[R68] 计算文件校验值
来源：http://hz.daria6918.cn/gtpzukvazs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj20258.top/gtosadhccy.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gtunphaqpt.html

head -c 16 /dev/urandom | base64
来源：http://hz.guowangkeji.top/gtaqfyfwxi.html

[R70] 时间戳与互转
来源：http://hz.andypj.xyz/gtbumyxuaz.html

date +%s;  date -d @1700000000
来源：http://hz.c1oappe.top/gtuxwtnndr.html

[R71] 日期格式化
来源：http://hz.zhixingplan.top/gtawlpppox.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtyvwautlv.html

[R72] 等待端口就绪
来源：http://hz.zhaomingkeji.xyz/gtzxyznnku.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.smart0.xyz/gthfvhnyte.html

[R73] 分割大日志
来源：http://hz.iojbl.cn/gtyogqdsuh.html

split -l 1000 big.log part_
来源：http://hz.xuanzx.com/gtqzzgxiju.html

[R74] 批量重命名
来源：http://hz.havefunace.top/gtbwspmyec.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ywan-chungtsiang.top/gtbnvykwto.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gttojpwnxp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xylfe.cn/gtpiwdfcxc.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtszadjkme.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtwdreglik.html

[R77] 读取用户输入
来源：http://hz.shuidangran.top/gttjkdpauj.html

read -rp "请输入: " ans
来源：http://hz.yj20258.top/gtknitjxxu.html

[R78] 交互式菜单
来源：http://hz.yj20258888.top/gtsxoywzic.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinqigufen.top/gtjloiygvi.html

[R79] 解析命令行选项
来源：http://hz.daxiang520.top/gtfkzaxirn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cheryme.top/gtcrklyudz.html

[R80] 查看脚本执行耗时
来源：http://hz.hfpthk.cn/gtujntlfyo.html

time ./run.sh
来源：http://hz.yj20258888.top/gtkaloxmpu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtpdzuuris.html

S. C / C++ 专题
来源：http://hz.xingfuxueyuan.xyz/gtpwigapxe.html

================================================================================
来源：http://hz.0kj1m.cn/gtzrbgxjyq.html

[S01] C：Hello World
来源：http://hz.jqgfzy.top/gteuedzxkr.html

#include <stdio.h>
来源：http://hz.nwbrower.top/gtsihtwbym.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.guowangkeji.top/gtbwtxevgp.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtasgdntyh.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258888.top/gtzucxsewf.html

[S03] C：读入整数
来源：http://hz.316326.xyz/gteeiogzwh.html

int x; scanf("%d", &x);
来源：http://hz.yonumen.top/gtvybxwcex.html

[S04] C：字符串复制
来源：http://hz.cqqwz.cn/gtyujyhyut.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtthtfqhku.html

[S05] C：字符串长度
来源：http://hz.jianghu66.top/gtmpmmuxwz.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gtbuiqorcf.html

[S06] C：字符串比较
来源：http://hz.xuetiantiany.cn/gtuyzvullq.html

strcmp(a, b) == 0
来源：http://hz.zhaomingkeji.xyz/gtdixoetjm.html

[S07] C：数组遍历求和
来源：http://hz.yuanzhike.top/gtbugjibqd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.vqdsnc.cn/gtfcddiofd.html

[S08] C：动态内存分配与释放
来源：http://hz.chenjidiqi.icu/gtimszfply.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgufenzy.top/gtexqrirub.html

[S09] C：结构体定义与初始化
来源：http://hz.sxryk.cn/gttyerxdji.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhijiandao.cn/gtpleldtgh.html

[S10] C：指针与解引用
来源：http://hz.jyoumei.cn/gtugxlkihx.html

int *p = &a;  *p = 5;
来源：http://hz.ppjwa.cn/gtqivevbrk.html

[S11] C：逐行读文件
来源：http://hz.jianghu66.top/gtqyhdvknb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtacmytruo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.svipenyu.cn/gtluvgbenr.html

fclose(f);
来源：http://hz.haohaochexian.top/gtozarbslp.html

[S12] C：写文件
来源：http://hz.yangfankeji.com/gtjtwhpsfp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuanzhike.top/gtmrerfscw.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtcjawmhmg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.mhx1999.top/gtwswwwask.html

[S14] C：枚举
来源：http://hz.yongpay.top/gtlvktriem.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gtrwmbvhae.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gtenhvpbxc.html

(double) a / b
来源：http://hz.ybcxt.top/gtodsqsqfm.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtubbgmoqp.html

x |= (1 << 3);
来源：http://hz.bjfxy.top/gtocfqhane.html

[S17] C：安全拼接字符串
来源：http://hz.vqdsnc.cn/gttqsghohj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jyoumei.cn/gtrituqchi.html

[S18] C：命令行参数
来源：http://hz.xuetiantiany.cn/gteitxnirw.html

int main(int argc, char **argv)
来源：http://hz.aibaodan.cn/gtqpgqdnrk.html

[S19] C：快速排序
来源：http://hz.zhiwuduotai.top/gtwvzzdmgy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtyvxuennr.html

[S20] C：二分查找
来源：http://hz.zhengqikj.top/gtatoctrvu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtbvcordet.html

[S21] C：字符类别判断
来源：http://hz.ywan-chungtsiang.top/gtkdauppdw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yuxming.cn/gtoonohcwm.html

[S22] C：字符串转数字
来源：http://hz.xinyue.icu/gtnvasvchq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtpafanowb.html

[S23] C：随机数
来源：http://hz.shzxlz.cn/gtosgowcje.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ybcxt.top/gtqcgdjajv.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gtaxjosdag.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuxming.cn/gtrwgbutzz.html

[S25] C：内存拷贝
来源：http://hz.dashuyun.cn/gtvtggaaua.html

memcpy(dst, src, n);
来源：http://hz.hywenlv.cn/gtwkfiawgj.html

[S26] C：内存清零
来源：http://hz.feifeiyinyue.top/gtajsozswa.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtedscngrw.html

[S27] C：定义常量
来源：http://hz.sweek.top/gtkafnsxpf.html

const double PI = 3.14159;
来源：http://hz.bjfxy.top/gtbkrjrrvi.html

[S28] C：静态变量
来源：http://hz.haohaochexian.top/gtkcikxjgg.html

static int counter = 0;
来源：http://hz.cashguo.top/gthblmapsy.html

[S29] C：变参函数
来源：http://hz.yongpay.top/gtfmnwtoks.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gtsrdhatqs.html

[S30] C：头文件保护
来源：http://hz.hammf.cn/gtroiriqkg.html

#ifndef X_H
来源：http://hz.ywan-chungtsiang.top/gtihvewzmr.html

#define X_H
来源：http://hz.xziqi.cn/gtaslqzcpb.html

#endif
来源：http://hz.yanxiufei.cn/gtfnldvabk.html

[S31] C++：Hello World
来源：http://hz.cucudq.cn/gttdqptowp.html

#include <iostream>
来源：http://hz.fengsongda.top/gttijbjlwy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.feifeiyinyue.top/gtrhmwafks.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtweywulgt.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxinkj.top/gtkhhwohho.html

[S33] C++：vector 增删
来源：http://hz.aizwys.cn/gtksghgemx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nwbrower.top/gtzwcbbqlo.html

[S34] C++：遍历 vector
来源：http://hz.wangshuangyany.cn/gtparodzld.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuxming.cn/gtbzuypdem.html

[S35] C++：map
来源：http://hz.shanyushiyangtech.top/gtwxeuefxd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtlzeonqrh.html

[S36] C++：unordered_map
来源：http://hz.quarkkingdee.top/gtbzekfaub.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gthqqqmwqe.html

[S37] C++：set
来源：http://hz.jianghu66.top/gtxksvxfgb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj20258.top/gtygmvufcr.html

[S38] C++：排序
来源：http://hz.gzhubu.top/gtqxcineez.html

std::sort(v.begin(), v.end());
来源：http://hz.zhaomingkeji.xyz/gtqdospfkt.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gtuspmdysw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sweek.top/gtqgifrgai.html

[S40] C++：查找元素
来源：http://hz.ybcxt.top/gtnkelllvy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtqwyxuxii.html

[S41] C++：类与构造函数
来源：http://hz.gaohongyu789.top/gtujaifnab.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydzc1.top/gtrjhtxzax.html

[S42] C++：继承与虚函数
来源：http://hz.ivvv.top/gtwahvgrxt.html

class B : public Base { public: void f() override {} };
来源：http://hz.fzhhl.top/gtngdfinlj.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gtqnzxfcys.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxuanxn.top/gtgfuljqwr.html

[S44] C++：引用传参
来源：http://hz.zdqjudy.top/gtovrpdmnc.html

void inc(int &x) { ++x; }
来源：http://hz.snrcjt.cn/gtvhtahvat.html

[S45] C++：lambda
来源：http://hz.guannengcc.top/gtzfwwzfkc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gteblqokog.html

[S46] C++：函数模板
来源：http://hz.snrcjt.cn/gtoymhecrp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydjk.org.cn/gtfqepgyor.html

[S47] C++：结构化绑定遍历
来源：http://hz.guowangkeji.top/gtxtxnmwvj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ywan-chungtsiang.top/gtsfyuuuir.html

[S48] C++：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtovvkesyj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pycfn.com/gttndphvup.html

while (std::getline(in, line)) { }
来源：http://hz.guowangkeji.top/gtbnrsykor.html

[S49] C++：写文件
来源：http://hz.zycfv.cn/gtpbhmpibp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.wangdashe.top/gtanmrnnxv.html

[S50] C++：格式化数字
来源：http://hz.0kj1m.cn/gtdkqklafv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fengsongda.top/gtousacogn.html

[S51] C++：显式类型转换
来源：http://hz.ydjk.org.cn/gtnealuqdz.html

static_cast<double>(a) / b
来源：http://hz.kuanghao11.cn/gtxkoymevh.html

[S52] C++：const 与 noexcept
来源：http://hz.sufxvd.cn/gtgbxnqnme.html

int size() const noexcept { return n_; }
来源：http://hz.ywan-chungtsiang.top/gtcomxqmwy.html

[S53] C++：移动语义
来源：http://hz.jinghuilouyu.cn/gtyvdrtyxy.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258888.top/gtzqxbmnvs.html

[S54] C++：异常处理
来源：http://hz.wangshuangyany.cn/gtrbzideja.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydjk.org.cn/gtrhzkpivv.html

[S55] C++：结构化绑定
来源：http://hz.ivvv.top/gtpfkegrnc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgufenzy.top/gtlphnjyqv.html

[S56] C++：optional
来源：http://hz.yvedp.cn/gtnnrjmych.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shzxlz.cn/gtcxhnedys.html

[S57] C++：编译期常量
来源：http://hz.feifeiyinyue.top/gtzagfmleu.html

constexpr int N = 10;
来源：http://hz.jyoumei.cn/gtvngimekd.html

[S58] C++：命名空间
来源：http://hz.cucudq.cn/gttqynclam.html

namespace ns { int f() { return 1; } }
来源：http://hz.cqqwz.cn/gtcvwphasb.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtevkdnuhe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gzhubu.top/gtwbokcvsu.html

[S60] C++：遍历并删除元素
来源：http://hz.hongshengwenyu.top/gtujxaogxn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cashguo.top/gtxjedfydj.html

================================================================================
来源：http://hz.wangdashe.top/gtvocjzytm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gtmbyzfuyh.html

================================================================================
来源：http://hz.zhijiandao.cn/gtajhgwlzc.html

[T01] Kotlin：Hello World
来源：http://hz.cqqwz.cn/gtrtyoaokd.html

println("Hello")
来源：http://hz.yangfankeji.com/gtqkztslmc.html

[T02] Kotlin：变量
来源：http://hz.shzxlz.cn/gtobisspbu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gtfvipwelw.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtacthkumx.html

"值: $b"
来源：http://hz.feifeiyinyue.top/gtrqyuymni.html

[T04] Kotlin：空安全
来源：http://hz.yvedp.cn/gtolwzoeoj.html

val n: String? = null;  n?.length
来源：http://hz.cashguo.top/gtgkqxkdvj.html

[T05] Kotlin：when 表达式
来源：http://hz.nwbrower.top/gtrarsllho.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gogol.net.cn/gtdvfdmzdi.html

[T06] Kotlin：集合映射
来源：http://hz.pycfn.com/gtpeqbxrvm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtehsrxomn.html

[T07] Kotlin：集合过滤
来源：http://hz.hysaishi.cn/gtzlutxgtr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydzc1.top/gteansumqh.html

[T08] Kotlin：数据类
来源：http://hz.hywenlv.cn/gtrehmwkvh.html

data class User(val name: String, val age: Int)
来源：http://hz.c1oappe.top/gtxljebraz.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gtwzhrtabp.html

fun String.exclaim() = this + "!"
来源：http://hz.sxryk.cn/gtbtvofdcl.html

[T10] Kotlin：默认参数
来源：http://hz.pengpengdd.cyou/gtyxjdagfm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yvedp.cn/gtmkyvoeeo.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtxwwzbexw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hywenlv.cn/gtuyjmbpxy.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtqnkusnzf.html

val (a, b) = Pair(1, 2)
来源：http://hz.yongpay.top/gtczdkixau.html

[T13] Kotlin：只读 Map
来源：http://hz.havefunace.top/gtwjqcqnow.html

val m = mapOf("a" to 1)
来源：http://hz.haohaochexian.top/gtjhhqkdic.html

[T14] Kotlin：循环
来源：http://hz.aibaodan.cn/gtyfrbesni.html

for (i in 1..10) println(i)
来源：http://hz.zdqjudy.top/gtddbcayyz.html

[T15] Kotlin：接口
来源：http://hz.sweek.top/gtfwzmrbnp.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gthdeyhvgf.html

[T16] Swift：Hello World
来源：http://hz.pengpengdd.cyou/gtdvbqoaha.html

print("Hello")
来源：http://hz.jianghu66.top/gtavefvqop.html

[T17] Swift：变量与常量
来源：http://hz.wangdashe.top/gtzchuhpfn.html

var a = 1;  let b = 2
来源：http://hz.yuxming.cn/gtffwznfoo.html

[T18] Swift：字符串插值
来源：http://hz.fengsongda.top/gtvnyoxknp.html

"值: \(b)"
来源：http://hz.hammf.cn/gtelkravjy.html

[T19] Swift：可选绑定
来源：http://hz.wangshuangyany.cn/gtmqbgwcbt.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtflzlcbzn.html

[T20] Swift：数组操作
来源：http://hz.xylfe.cn/gtgaorxuto.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yvedp.cn/gtefhctcjk.html


<!-- 参考信息 -->