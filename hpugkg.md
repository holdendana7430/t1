代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yongpay.top/gttyqrpthn.html

[R16] until 等待条件
来源：http://hz.hnqzz.top/gtuiwmksee.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gzhubu.top/gtrkszgnyo.html

[R17] 数组定义与取值
来源：http://hz.shzxlz.cn/gtkeigwscb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.0kj1m.cn/gtdjvykxou.html

[R18] 遍历数组
来源：http://hz.gotoacloud.top/gtdmnsvsqx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tanke756.top/gthbvktdzp.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtvhkcoczu.html

echo "${#arr[@]}"
来源：http://hz.fzhhl.top/gtufbkmtos.html

[R20] 关联数组（字典）
来源：http://hz.svipenyu.cn/gtbzfrjadw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ywan-chungtsiang.top/gtcvnmtkii.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gtcrbyrlae.html

echo "${#s}"
来源：http://hz.tian-w.cn/gtjtwlwapr.html

[R22] 截取子串
来源：http://hz.xziqi.cn/gteifxuaki.html

echo "${s:0:5}"
来源：http://hz.aibaodan.cn/gtynnchdhb.html

[R23] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtqtcyfvzh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydjk.org.cn/gtyfqhdiic.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtnxviwjry.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jiagoushi.top/gtwdmjbygt.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhengqikj.top/gtujeqnhkt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cucudq.cn/gtoddxxseg.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtbsubgeat.html

now=$(date +%F); echo "$now"
来源：http://hz.bjfxy.top/gtrgfvixau.html

[R27] 算术展开
来源：http://hz.ybcxt.top/gtxjgocodo.html

echo $((1 + 2 * 3))
来源：http://hz.hysaishi.cn/gtxbkpkvcz.html

[R28] 浮点运算
来源：http://hz.sweek.top/gtuzynnctw.html

echo "scale=2; 10/3" | bc
来源：http://hz.jqgufenzy.top/gtafzjwmuc.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gtjdudhtnp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.andypj.xyz/gtjzmvjwqv.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtadualxth.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.kuanghao11.cn/gtikrxmboi.html

[R31] 局部变量
来源：http://hz.c1oappe.top/gtutitaipg.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj20258888.top/gtpoferqlh.html

[R32] 参数个数校验
来源：http://hz.haohaochexian.top/gtrugdjrwv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258.top/gtjdfgrgbl.html

[R33] 捕获错误并提示行号
来源：http://hz.sufxvd.cn/gtzoljbtki.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hongshengwenyu.top/gtatnrmqqn.html

[R34] 退出时清理
来源：http://hz.52xcode.cn/gtqetgftlp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtgzvdxdeh.html

[R35] 后台执行并等待
来源：http://hz.vqdsnc.cn/gtqshibftn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgfzy.top/gtwmumdpyf.html

[R36] 并发执行多个任务
来源：http://hz.sweek.top/gttkhjhucz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cheryme.top/gtxyrfztue.html

[R37] 把输出赋给变量
来源：http://hz.yj20258888.top/gtwqvqclkl.html

files=$(ls -1)
来源：http://hz.guowangkeji.top/gtbbtfleir.html

[R38] 管道串联
来源：http://hz.cdnleiting.top/gtuewwpqgd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dashuyun.cn/gtrxlzksqp.html

[R39] 重定向标准输出与错误
来源：http://hz.yuxming.cn/gtwicwexce.html

cmd > out.log 2>&1
来源：http://hz.chenzaomai.com/gtrgpbgdje.html

[R40] 追加写日志
来源：http://hz.hammf.cn/gtbnhpylyv.html

echo "log" >> out.log
来源：http://hz.hammf.cn/gtrurocmii.html

[R41] 丢弃输出
来源：http://hz.andypj.xyz/gtieumplrw.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gttoavrrdh.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gtneiqqwma.html

wc -l < a.txt
来源：http://hz.hfpthk.cn/gtnifgvqzt.html

[R43] 按名字查找文件
来源：http://hz.xziqi.cn/gtbzxoskmw.html

find . -name "*.log" -type f
来源：http://hz.guowangkeji.top/gtiifhmqwh.html

[R44] 按修改时间查找
来源：http://hz.xuetiantiany.cn/gtjtdumdqi.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangtech.top/gttylikfgn.html

[R45] 批量删除
来源：http://hz.52xcode.cn/gtaebvvilm.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtkujzonrs.html

[R46] 递归替换文件内容
来源：http://hz.tanke756.top/gtjzeqqkpg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.quarkkingdee.top/gtpaggorqm.html

[R47] sed 单行替换
来源：http://hz.sufxvd.cn/gtymwdpmsq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shanyushiyangtech.top/gtgdxxbwhp.html

[R48] awk 取指定列
来源：http://hz.yongpay.top/gtuvgtdpfx.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhixingplan.top/gtqbvqhpfm.html

[R49] awk 带条件
来源：http://hz.wangdashe.top/gtldhdjagl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gogol.net.cn/gtphleracl.html

[R50] awk 求和
来源：http://hz.zhixingplan.top/gtiqnzpazo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ehwqpu.com/gtqsgqkrnh.html

[R51] 排序去重取前几
来源：http://hz.ydzc1.top/gtawrowmry.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.mhx1999.top/gtohiecuul.html

[R52] 统计行数
来源：http://hz.xingfuxueyuan.xyz/gtkmhilfsv.html

wc -l a.txt
来源：http://hz.quarkkingdee.top/gtspooputg.html

[R53] 查看文件头与实时尾
来源：http://hz.jyoumei.cn/gtlvxfhfhg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigfzy.top/gtyhpjclxi.html

[R54] 比较两个文件
来源：http://hz.daria6918.cn/gteozbhkha.html

diff a.txt b.txt
来源：http://hz.cqqwz.cn/gtllqdbfxk.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtstslyspx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhongyouzk.top/gtrezbtrfj.html

[R56] 远程拷贝
来源：http://hz.guannengcc.top/gtkkkdliem.html

scp file user@host:/path/
来源：http://hz.shuidangran.top/gtduqygxgv.html

[R57] 远程执行命令
来源：http://hz.tianlin.xyz/gtampsxwov.html

ssh user@host 'uptime'
来源：http://hz.zhaomingkeji.xyz/gtylugbjhb.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtoqsqkqkb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtupyqaloy.html

[R59] 发 POST JSON
来源：http://hz.smart0.xyz/gtcurddolj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gzhubu.top/gtsoimuvbn.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gtbhyyhqfu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangshuangyany.cn/gtwgdryvap.html

[R61] 磁盘占用
来源：http://hz.sxryk.cn/gtdcrzxmxf.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtvciiufbz.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gtbcodkxwh.html

du -ah . | sort -rh | head -10
来源：http://hz.ybcxt.top/gtmjnqwvon.html

[R63] 内存与进程
来源：http://hz.xylfe.cn/gtjpkpkjtx.html

free -h;  ps aux | grep nginx
来源：http://hz.sweek.top/gtgokrqfrz.html

[R64] 结束进程
来源：http://hz.zhiwuduotai.top/gtdqoycqra.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sweek.top/gtqmrmfats.html

[R65] 查看端口占用
来源：http://hz.fengsongda.top/gtcsuicigw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sufxvd.cn/gtpamtebzs.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtkbqsvoad.html

crontab -e;  crontab -l
来源：http://hz.cqqwz.cn/gtjbkrpjsc.html

[R67] 生成随机十六进制串
来源：http://hz.ydzc1.top/gtbmsjekjj.html

openssl rand -hex 16
来源：http://hz.gogol.net.cn/gtwzizsskl.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtkyiiofsc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aizwys.cn/gtawhjxlzj.html

[R69] 生成随机密码
来源：http://hz.bjfxy.top/gtbmtscvyo.html

head -c 16 /dev/urandom | base64
来源：http://hz.ppjwa.cn/gtrwcxfqww.html

[R70] 时间戳与互转
来源：http://hz.cucudq.cn/gtpzljzptu.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtnmamjyia.html

[R71] 日期格式化
来源：http://hz.ivvv.top/gtdwkethll.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuanzx.com/gtzaagidjo.html

[R72] 等待端口就绪
来源：http://hz.shzxlz.cn/gtougjsmps.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtalfepxbx.html

[R73] 分割大日志
来源：http://hz.cucudq.cn/gtxmvjjhlk.html

split -l 1000 big.log part_
来源：http://hz.yanxiufei.cn/gtekbltmyg.html

[R74] 批量重命名
来源：http://hz.hammf.cn/gtygziqkwq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xylfe.cn/gtgjaarcek.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtedfyorrf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnxiangtu.top/gttyammnfu.html

[R76] 使用临时文件
来源：http://hz.yj20258.top/gtzaiisbub.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gteewrxqfz.html

[R77] 读取用户输入
来源：http://hz.pycfn.com/gtlivoizuh.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gtrquzeurh.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtymzpgkve.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangkeji.top/gtibfmmglt.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gtwinaswyd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shangyingyoupin.top/gtissrwrwn.html

[R80] 查看脚本执行耗时
来源：http://hz.ydzc1.top/gtgvjlrbly.html

time ./run.sh
来源：http://hz.hysaishi.cn/gtbbnupxia.html

================================================================================
来源：http://hz.sysykeji.top/gtwxymsgzp.html

S. C / C++ 专题
来源：http://hz.cheryme.top/gtgmcozblk.html

================================================================================
来源：http://hz.aizwys.cn/gtbpkmaohe.html

[S01] C：Hello World
来源：http://hz.zhoulong.xyz/gtaieqkrdv.html

#include <stdio.h>
来源：http://hz.nanxuanxn.top/gtrhboexjr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.0kj1m.cn/gtebmiyncg.html

[S02] C：变量与格式化输出
来源：http://hz.zhoulong.xyz/gtuaetmdwv.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhengqikj.top/gtvhmmqvmb.html

[S03] C：读入整数
来源：http://hz.hnxiangtu.top/gteiqfjqsg.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gtyvyycloo.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtbtsmykpp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.0kj1m.cn/gttujsfrtp.html

[S05] C：字符串长度
来源：http://hz.birdmap.top/gtdcxysmnm.html

strlen(s)
来源：http://hz.ehwqpu.com/gtjjdjxbiz.html

[S06] C：字符串比较
来源：http://hz.yj20258.top/gtkeirsufy.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtummzxumw.html

[S07] C：数组遍历求和
来源：http://hz.yj20258.top/gtibjcfadt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxinkj.top/gtvorlkoic.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtjtglygla.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtmbjkqrbd.html

[S09] C：结构体定义与初始化
来源：http://hz.andypj.xyz/gtuhjivzmm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenlongwang.top/gtbswrpuvg.html

[S10] C：指针与解引用
来源：http://hz.cheryme.top/gtltkzrpbr.html

int *p = &a;  *p = 5;
来源：http://hz.pycfn.com/gtaecdujkq.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtdisrvwxs.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yonumen.top/gtnkzuorwz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dashuyun.cn/gtuxvhvsqa.html

fclose(f);
来源：http://hz.bjfxy.top/gtuepwuhxp.html

[S12] C：写文件
来源：http://hz.svipenyu.cn/gtlzdbmdqp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinqigfzy.top/gtgkkxwrhd.html

[S13] C：宏定义
来源：http://hz.havefunace.top/gtaumxtzgs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hfpthk.cn/gtyejsbecc.html

[S14] C：枚举
来源：http://hz.shzxlz.cn/gtxrbqpzis.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.kuanghao11.cn/gtsuqtfjqi.html

[S15] C：类型转换
来源：http://hz.andypj.xyz/gtbxjcvmdx.html

(double) a / b
来源：http://hz.jianghu66.top/gtdfwyytfx.html

[S16] C：位操作置位
来源：http://hz.zhiwuduotai.top/gtjlhdggxc.html

x |= (1 << 3);
来源：http://hz.gogol.net.cn/gtsxhakwao.html

[S17] C：安全拼接字符串
来源：http://hz.pycfn.com/gtymopxgvk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnxiangtu.top/gtlrdlbkvc.html

[S18] C：命令行参数
来源：http://hz.9152youxi.cn/gtmhvvzpgm.html

int main(int argc, char **argv)
来源：http://hz.iojbl.cn/gtwvoacqql.html

[S19] C：快速排序
来源：http://hz.bjfxy.top/gtmqmvsokz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtxuunfkzj.html

[S20] C：二分查找
来源：http://hz.wangdashe.top/gtfefgbjjy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gtjwdovrsd.html

[S21] C：字符类别判断
来源：http://hz.zhixingplan.top/gtvbwfzcor.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigfzy.top/gtgmccyvmd.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtpmbsutup.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jyoumei.cn/gtapfsfgqx.html

[S23] C：随机数
来源：http://hz.ydzc1.top/gtmqbqxycs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtnthemqfz.html

[S24] C：获取本地时间
来源：http://hz.zhongyouzk.top/gtmlgvaxwg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtnnssasmi.html

[S25] C：内存拷贝
来源：http://hz.xziqi.cn/gtrhezlkrt.html

memcpy(dst, src, n);
来源：http://hz.yvedp.cn/gtmewsrxza.html

[S26] C：内存清零
来源：http://hz.nanxuanxn.top/gtduyclxdd.html

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangkeji.top/gtzswkpcxu.html

[S27] C：定义常量
来源：http://hz.dashuyun.cn/gtzksjwmjh.html

const double PI = 3.14159;
来源：http://hz.fengsongda.top/gtiwmkwlbi.html

[S28] C：静态变量
来源：http://hz.shzxlz.cn/gtejnaftht.html

static int counter = 0;
来源：http://hz.shangyingyoupin.top/gtpewhypnl.html

[S29] C：变参函数
来源：http://hz.kuanghao11.cn/gtvxucboep.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jyoumei.cn/gtmwfnsnki.html

[S30] C：头文件保护
来源：http://hz.sxryk.cn/gtiieslgpx.html

#ifndef X_H
来源：http://hz.smart0.xyz/gtocfjnpzr.html

#define X_H
来源：http://hz.vqdsnc.cn/gtbpqtnuda.html

#endif
来源：http://hz.zhengqikj.top/gtmrklzqdo.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gthqmlwzuh.html

#include <iostream>
来源：http://hz.kuanghao11.cn/gthuefkkth.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shangyingyoupin.top/gtgdwiaebh.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtigwfvumg.html

std::string s = "hi";  s += "!";
来源：http://hz.aizwys.cn/gtiaejgvcy.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtyegqcbuq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xinyue.icu/gtwkieadha.html

[S34] C++：遍历 vector
来源：http://hz.wangdashe.top/gtamiucabd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yanxiufei.cn/gtivbbqzjv.html

[S35] C++：map
来源：http://hz.sysykeji.top/gtzyiyeich.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gttbclmzcc.html

[S36] C++：unordered_map
来源：http://hz.zhoulong.xyz/gtquehimiw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guowangkeji.top/gtskogrhiw.html

[S37] C++：set
来源：http://hz.hysaishi.cn/gttzeiafnm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenjidiqi.icu/gthdbwjdkb.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtfmzhfyax.html

std::sort(v.begin(), v.end());
来源：http://hz.gotoacloud.top/gtjykscxej.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtmutvqzgz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtwncgwlqo.html

[S40] C++：查找元素
来源：http://hz.zhongyouzk.top/gtthjjwaru.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.redwolf501.top/gtqvqlhfyb.html

[S41] C++：类与构造函数
来源：http://hz.bjfxy.top/gtrydnuyoe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gtonygaucn.html

[S42] C++：继承与虚函数
来源：http://hz.shzxlz.cn/gtchwjxagi.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gtfxmgpefs.html

[S43] C++：智能指针
来源：http://hz.snrcjt.cn/gtnganswfp.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuxming.cn/gtybgyejxh.html

[S44] C++：引用传参
来源：http://hz.sxryk.cn/gteohvcejp.html

void inc(int &x) { ++x; }
来源：http://hz.tanke756.top/gtzrduqmlp.html

[S45] C++：lambda
来源：http://hz.shuidangran.top/gtitnvynpj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shuidangran.top/gtrsvxhzhy.html

[S46] C++：函数模板
来源：http://hz.quarkkingdee.top/gtrrmwycpj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.haohaochexian.top/gtfftefzzr.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhongyouzk.top/gtiyboygjb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daxiang520.top/gtporknegh.html

[S48] C++：逐行读文件
来源：http://hz.sxryk.cn/gtpdxlyjrd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yvedp.cn/gtbunsddiq.html

while (std::getline(in, line)) { }
来源：http://hz.xylfe.cn/gtxczelxrc.html

[S49] C++：写文件
来源：http://hz.yangfankeji.com/gtbxefdjsv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenlongwang.top/gtnezzbdxk.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gtxtdmrvgt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gaohongyu789.top/gtzyctwuad.html

[S51] C++：显式类型转换
来源：http://hz.nanxuanxn.top/gtvwcglfwn.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtlwoemlzy.html

[S52] C++：const 与 noexcept
来源：http://hz.snrcjt.cn/gtdnuajccd.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gtzuytbmdx.html

[S53] C++：移动语义
来源：http://hz.jinqigfzy.top/gtvxpyjxya.html

std::vector<int> w = std::move(v);
来源：http://hz.0kj1m.cn/gtozqifqyx.html

[S54] C++：异常处理
来源：http://hz.zycfv.cn/gtythukycq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhixingplan.top/gtvjpynprp.html

[S55] C++：结构化绑定
来源：http://hz.guannengcc.top/gtyhiovhvp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ybcxt.top/gtmrgfwubd.html

[S56] C++：optional
来源：http://hz.gogol.net.cn/gtesyreuuw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtrcjynzlh.html

[S57] C++：编译期常量
来源：http://hz.jqgfzy.top/gthdflsxfn.html

constexpr int N = 10;
来源：http://hz.hnqzz.top/gtwnnlfczm.html

[S58] C++：命名空间
来源：http://hz.bjfxy.top/gtagaybwie.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxinkj.top/gtncncktgt.html

[S59] C++：静态断言
来源：http://hz.shuidangran.top/gtibddzmkq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pengpengdd.cyou/gtlrrghori.html

[S60] C++：遍历并删除元素
来源：http://hz.haohaochexian.top/gtmpqptbax.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhiwuduotai.top/gttiwifjez.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthdglerqc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dashuyun.cn/gtlrqrlfzx.html

================================================================================
来源：http://hz.zdqjudy.top/gtqitjqufa.html

[T01] Kotlin：Hello World
来源：http://hz.jianghu66.top/gtitywfurp.html

println("Hello")
来源：http://hz.pengpengdd.cyou/gtgplhdizq.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtratuqsed.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.snrcjt.cn/gtyvonhxki.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangtech.top/gtkoigtqcc.html

"值: $b"
来源：http://hz.fengsongda.top/gtedtegpbm.html

[T04] Kotlin：空安全
来源：http://hz.pengpengdd.cyou/gtvfjbrnpw.html

val n: String? = null;  n?.length
来源：http://hz.chenjidiqi.icu/gtpclzewzo.html

[T05] Kotlin：when 表达式
来源：http://hz.andypj.xyz/gtttwyophz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtlwjpeleb.html

[T06] Kotlin：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtdlrcvdba.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cqqwz.cn/gtjtsugoun.html

[T07] Kotlin：集合过滤
来源：http://hz.sxryk.cn/gthevrpwzd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jqgfzy.top/gtdojhikif.html

[T08] Kotlin：数据类
来源：http://hz.xuetiantiany.cn/gtcfymwnkl.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gthycxsdlm.html

[T09] Kotlin：扩展函数
来源：http://hz.fengsongda.top/gtamxmbuid.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtaclgnvxz.html

[T10] Kotlin：默认参数
来源：http://hz.andypj.xyz/gtpqcbpsca.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtpvzvrndi.html

[T11] Kotlin：协程
来源：http://hz.cashguo.top/gtafjlwwen.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.meibo888.top/gtldrzpqdk.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gtxrtguxot.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gtornaldcb.html

[T13] Kotlin：只读 Map
来源：http://hz.pengpengdd.cyou/gthjzhvput.html

val m = mapOf("a" to 1)
来源：http://hz.dashuyun.cn/gtkrczxtmx.html

[T14] Kotlin：循环
来源：http://hz.svipenyu.cn/gtsuhhrvly.html

for (i in 1..10) println(i)
来源：http://hz.dashuyun.cn/gtferguuqh.html

[T15] Kotlin：接口
来源：http://hz.feifeiyinyue.top/gtixnkrrni.html

interface Shape { fun area(): Double }
来源：http://hz.zhengqikj.top/gtkbwybrai.html

[T16] Swift：Hello World
来源：http://hz.dianchejie.cn/gtgdxltpog.html

print("Hello")
来源：http://hz.zhixingplan.top/gtneafvjix.html

[T17] Swift：变量与常量
来源：http://hz.yj20258888.top/gtinexzvyj.html

var a = 1;  let b = 2
来源：http://hz.haohaochexian.top/gtcnrdkona.html

[T18] Swift：字符串插值
来源：http://hz.nanxinkj.top/gtamenekta.html

"值: \(b)"
来源：http://hz.dianchejie.cn/gtevuygtre.html


<!-- 参考信息 -->