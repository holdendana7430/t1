代发 wailian999

readonly PI=3.14
来源：http://hz.yj20258888.top/gtlxhjdhih.html

[R04] 位置参数
来源：http://hz.xuetiantiany.cn/gtvscytwdq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hammf.cn/gtggwzlbur.html

[R05] 参数默认值
来源：http://hz.yj20258888.top/gtuzyzkafs.html

name="${1:-default}"
来源：http://hz.yj20258888.top/gtqbslopdz.html

[R06] 判断命令是否存在
来源：http://hz.chenjidiqi.icu/gtfojlenxa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daxiang520.top/gtrkvjrqir.html

[R07] if 判断文件
来源：http://hz.xziqi.cn/gtgwidvgqe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jqgfzy.top/gtkemidtoc.html

[R08] 数值比较
来源：http://hz.ivvv.top/gtucjwkdsd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gtbiilzreg.html

[R09] 字符串比较
来源：http://hz.52xcode.cn/gtytmobdrd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhixingplan.top/gtfidyoudw.html

[R10] 正则匹配
来源：http://hz.wangshuangyany.cn/gtoemsvzal.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gtzqrpttvf.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtgjnqiauk.html

case "$1" in
来源：http://hz.birdmap.top/gtlogmzjaj.html

start) echo "启动" ;;
来源：http://hz.yongpay.top/gtpkanwxtv.html

stop)  echo "停止" ;;
来源：http://hz.ivvv.top/gtnqjwbodc.html

*)     echo "未知命令" ;;
来源：http://hz.tian-w.cn/gtaycxdtpb.html

esac
来源：http://hz.nanxinkj.top/gttjbciqyx.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangkeji.top/gtqqmfoykm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnxiangtu.top/gtwxudehvi.html

[R13] for 计数循环
来源：http://hz.xinyue.icu/gtbcesqvme.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fzhhl.top/gtxntorjwy.html

[R14] C 风格 for
来源：http://hz.sufxvd.cn/gtehmeqqbt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuanzx.com/gtxpnvnwnh.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gtwvwxkbfb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.52xcode.cn/gtqmnlfzkp.html

[R16] until 等待条件
来源：http://hz.yonumen.top/gtmvxvmkwv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gttypgvzgl.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtqpsmyaii.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhaomingkeji.xyz/gtknfazpof.html

[R18] 遍历数组
来源：http://hz.haohaochexian.top/gtutvhwcby.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtdierjyll.html

[R19] 数组长度
来源：http://hz.yonumen.top/gtzmgykvaw.html

echo "${#arr[@]}"
来源：http://hz.chenzaomai.com/gtzqooicdg.html

[R20] 关联数组（字典）
来源：http://hz.iojbl.cn/gtjzcvimpk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xylfe.cn/gtwwryhmcx.html

[R21] 字符串长度
来源：http://hz.jqgufenzy.top/gtbddtjawe.html

echo "${#s}"
来源：http://hz.jinqigfzy.top/gtogakubpa.html

[R22] 截取子串
来源：http://hz.xinyue.icu/gtebzvgfdy.html

echo "${s:0:5}"
来源：http://hz.zhaomingkeji.xyz/gtqhocvmvd.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtopgymxil.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gtdxefytfv.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtzslyqnkw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gtcatyypmy.html

[R25] 去后缀 / 去前缀
来源：http://hz.dianchejie.cn/gtnxjjvxxl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shuidangran.top/gtzjlioulz.html

[R26] 命令替换
来源：http://hz.cdnleiting.top/gtgkxnjsmy.html

now=$(date +%F); echo "$now"
来源：http://hz.jianghu66.top/gtebonhafq.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtkfwibuyp.html

echo $((1 + 2 * 3))
来源：http://hz.fzhhl.top/gtsxjjqprf.html

[R28] 浮点运算
来源：http://hz.hammf.cn/gtucesiehi.html

echo "scale=2; 10/3" | bc
来源：http://hz.haohaochexian.top/gtkvsoradj.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtoccjqiqq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuetiantiany.cn/gtuaohdvyx.html

[R30] 函数返回状态码
来源：http://hz.c1oappe.top/gtwxhzhcjt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuetiantiany.cn/gttxxvvznn.html

[R31] 局部变量
来源：http://hz.xinyue.icu/gtouhakurv.html

f() { local x=1; echo "$x"; }
来源：http://hz.sweek.top/gtibudsxku.html

[R32] 参数个数校验
来源：http://hz.ywan-chungtsiang.top/gtxqszegnv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtdsqljblt.html

[R33] 捕获错误并提示行号
来源：http://hz.zdqjudy.top/gtkuggdvkz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigfzy.top/gtdaeqtyhj.html

[R34] 退出时清理
来源：http://hz.feifeiyinyue.top/gtsrcytfod.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gthvttkwby.html

[R35] 后台执行并等待
来源：http://hz.ehwqpu.com/gtskkwkogz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtazavarns.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gthzfvubxy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtplxkavuj.html

[R37] 把输出赋给变量
来源：http://hz.xziqi.cn/gtfwxehgbc.html

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtuqmyehrb.html

[R38] 管道串联
来源：http://hz.guowangkeji.top/gtwwldavqc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gogol.net.cn/gtvqlbystr.html

[R39] 重定向标准输出与错误
来源：http://hz.gzhubu.top/gtlabaggoh.html

cmd > out.log 2>&1
来源：http://hz.hongshengwenyu.top/gtnopgoiic.html

[R40] 追加写日志
来源：http://hz.ywan-chungtsiang.top/gtofeodztv.html

echo "log" >> out.log
来源：http://hz.wangdashe.top/gtvltwnnky.html

[R41] 丢弃输出
来源：http://hz.fengsongda.top/gttlxyijix.html

cmd >/dev/null 2>&1
来源：http://hz.cashguo.top/gtbfpdbsad.html

[R42] 输入重定向
来源：http://hz.zhongyouzk.top/gtyhcqrepj.html

wc -l < a.txt
来源：http://hz.yueranfly.top/gtlijixtjb.html

[R43] 按名字查找文件
来源：http://hz.ivvv.top/gtxlasnsjo.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gtdvjcvisl.html

[R44] 按修改时间查找
来源：http://hz.birdmap.top/gtpvyoakyo.html

find . -mtime -7 -type f
来源：http://hz.smart0.xyz/gtfzbcehqk.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gttfniuggj.html

find . -name "*.tmp" -delete
来源：http://hz.aibaodan.cn/gttuhpdlqu.html

[R46] 递归替换文件内容
来源：http://hz.cheryme.top/gthekgcsua.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gotoacloud.top/gtqmvwbsva.html

[R47] sed 单行替换
来源：http://hz.vqdsnc.cn/gttxduhgww.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hnxiangtu.top/gttwqsviby.html

[R48] awk 取指定列
来源：http://hz.hywenlv.cn/gtllwwvcdh.html

awk '{print $1, $3}' a.txt
来源：http://hz.snrcjt.cn/gtvkdqogtz.html

[R49] awk 带条件
来源：http://hz.yuanzhike.top/gtdumwvidg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cucudq.cn/gtqkyeqpuk.html

[R50] awk 求和
来源：http://hz.gzhubu.top/gtlbzozzcd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.bjfxy.top/gtgkpgcrxx.html

[R51] 排序去重取前几
来源：http://hz.yangfankeji.com/gterrqhkmd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aizwys.cn/gtbmiephbx.html

[R52] 统计行数
来源：http://hz.52xcode.cn/gtwhpvpyka.html

wc -l a.txt
来源：http://hz.hongshengwenyu.top/gtfnftgehm.html

[R53] 查看文件头与实时尾
来源：http://hz.jinyuanbaomall.cn/gthejcoxyd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gtiuatcgcs.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtkrqfgsmk.html

diff a.txt b.txt
来源：http://hz.sufxvd.cn/gtlthrpmys.html

[R55] 压缩与解压
来源：http://hz.yonumen.top/gtvkmdyhkk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhoulong.xyz/gtzzeecgxb.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtuimsfpxm.html

scp file user@host:/path/
来源：http://hz.jinqigufen.top/gtenxpwzfz.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtolfqseyn.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtotzrazbn.html

[R58] 下载文件
来源：http://hz.aizwys.cn/gttiqufpvo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtwbiccnrk.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gtwnyeufme.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.birdmap.top/gtkvlyzdzm.html

[R60] 只看 HTTP 状态码
来源：http://hz.sysykeji.top/gtbqkdlcyg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydjk.org.cn/gttyzcqeuk.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtqoqnsfje.html

df -h;  du -sh *
来源：http://hz.birdmap.top/gtjwdwtrhj.html

[R62] 找最占空间的文件
来源：http://hz.fzhhl.top/gtoerdzjti.html

du -ah . | sort -rh | head -10
来源：http://hz.aizwys.cn/gtkdrjofbk.html

[R63] 内存与进程
来源：http://hz.hongshengwenyu.top/gtuytnfvdl.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtpqjrvmlr.html

[R64] 结束进程
来源：http://hz.hammf.cn/gtxytjtxzc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shuidangran.top/gthrszfibz.html

[R65] 查看端口占用
来源：http://hz.sweek.top/gtnrzuehco.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtuhfcoyia.html

[R66] 定时任务
来源：http://hz.cashguo.top/gtznbdszsq.html

crontab -e;  crontab -l
来源：http://hz.birdmap.top/gtftmoniwv.html

[R67] 生成随机十六进制串
来源：http://hz.jianghu66.top/gtzddizilx.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gtgnkdazxb.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtmdoqkbye.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.kuanghao11.cn/gtxxmyetef.html

[R69] 生成随机密码
来源：http://hz.daxiang520.top/gtafutnggl.html

head -c 16 /dev/urandom | base64
来源：http://hz.yongpay.top/gtzlxhqbwp.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtlffjrgdc.html

date +%s;  date -d @1700000000
来源：http://hz.ywan-chungtsiang.top/gthsdqivob.html

[R71] 日期格式化
来源：http://hz.gaohongyu789.top/gtvkqgwnye.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.andypj.xyz/gtlzlftzae.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtadosllzf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.redwolf501.top/gtxxhorjsx.html

[R73] 分割大日志
来源：http://hz.yuanzhike.top/gtmojyxbci.html

split -l 1000 big.log part_
来源：http://hz.sxryk.cn/gtphyocjnn.html

[R74] 批量重命名
来源：http://hz.svipenyu.cn/gtmpuknyuk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.smart0.xyz/gtwtywwxde.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtmrwuqfyw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gtxbrgwchc.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtqezveipf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtawbntykf.html

[R77] 读取用户输入
来源：http://hz.pengpengdd.cyou/gtwacfutak.html

read -rp "请输入: " ans
来源：http://hz.xuetiantiany.cn/gtxuhftxfa.html

[R78] 交互式菜单
来源：http://hz.fzhhl.top/gtrquxzdix.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dianchejie.cn/gtncxmuogl.html

[R79] 解析命令行选项
来源：http://hz.yj20258888.top/gtwaakjnmf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xinyue.icu/gtmksrakqp.html

[R80] 查看脚本执行耗时
来源：http://hz.kuanghao11.cn/gtklqeijva.html

time ./run.sh
来源：http://hz.shzxlz.cn/gtwojlackg.html

================================================================================
来源：http://hz.52xcode.cn/gtujijwhza.html

S. C / C++ 专题
来源：http://hz.cheryme.top/gtdkbibcyy.html

================================================================================
来源：http://hz.52xcode.cn/gtsaepscbn.html

[S01] C：Hello World
来源：http://hz.chenjidiqi.icu/gtnxvseovo.html

#include <stdio.h>
来源：http://hz.dianchejie.cn/gtlgyqqhif.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenzaomai.com/gtbephztpp.html

[S02] C：变量与格式化输出
来源：http://hz.316326.xyz/gtnrhozfez.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangtech.top/gtziubmcim.html

[S03] C：读入整数
来源：http://hz.zhoulong.xyz/gtuebnomct.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gtcfismcff.html

[S04] C：字符串复制
来源：http://hz.hnxiangtu.top/gtzjaapvkb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jiagoushi.top/gtubpmffze.html

[S05] C：字符串长度
来源：http://hz.cheryme.top/gtwyrefdes.html

strlen(s)
来源：http://hz.nanxuanxn.top/gturgkwgig.html

[S06] C：字符串比较
来源：http://hz.havefunace.top/gtytqossdn.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gthnfimzbu.html

[S07] C：数组遍历求和
来源：http://hz.zhoulong.xyz/gttrtcvera.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ppjwa.cn/gtpqqkctdq.html

[S08] C：动态内存分配与释放
来源：http://hz.yuanzhike.top/gtjshzaaky.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ivvv.top/gtsktjuagu.html

[S09] C：结构体定义与初始化
来源：http://hz.tanke756.top/gtvpaqskcy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cheryme.top/gtheucmjwp.html

[S10] C：指针与解引用
来源：http://hz.cucudq.cn/gtznqesblt.html

int *p = &a;  *p = 5;
来源：http://hz.jinyuanbaomall.cn/gtsiyzdbqa.html

[S11] C：逐行读文件
来源：http://hz.316326.xyz/gtxdsvvfco.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ybcxt.top/gtnzzwzwqr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigufen.top/gtuwfetelu.html

fclose(f);
来源：http://hz.zhiwuduotai.top/gtsdvslcuo.html

[S12] C：写文件
来源：http://hz.yj20258888.top/gtgsazasfk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinghuilouyu.cn/gtvdssmhyf.html

[S13] C：宏定义
来源：http://hz.redwolf501.top/gtgzpstwky.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.havefunace.top/gtmvcgkpez.html

[S14] C：枚举
来源：http://hz.fengsongda.top/gtnaukignd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxinkj.top/gtzbzkwmzo.html

[S15] C：类型转换
来源：http://hz.quarkkingdee.top/gtqvszpipb.html

(double) a / b
来源：http://hz.feifeiyinyue.top/gtecupeqaf.html

[S16] C：位操作置位
来源：http://hz.aibaodan.cn/gtmensbqvg.html

x |= (1 << 3);
来源：http://hz.kuanghao11.cn/gttvvjmdjj.html

[S17] C：安全拼接字符串
来源：http://hz.gzhubu.top/gtriaxglzi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.316326.xyz/gtmweeyrlj.html

[S18] C：命令行参数
来源：http://hz.chenjidiqi.icu/gtjqxnzbpl.html

int main(int argc, char **argv)
来源：http://hz.sysykeji.top/gtqeqprdgb.html

[S19] C：快速排序
来源：http://hz.yanxiufei.cn/gtmfrmkngp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtutkiiuou.html

[S20] C：二分查找
来源：http://hz.zhaomingkeji.xyz/gtsijppqaw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtzrlfmvin.html

[S21] C：字符类别判断
来源：http://hz.xuetiantiany.cn/gtbycvheas.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhixingplan.top/gtgfnhdlac.html

[S22] C：字符串转数字
来源：http://hz.0kj1m.cn/gtgbiuwmyf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.feifeiyinyue.top/gtxevboock.html

[S23] C：随机数
来源：http://hz.yuxming.cn/gtybpvscaz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.316326.xyz/gtxoqcrcag.html

[S24] C：获取本地时间
来源：http://hz.yonumen.top/gtbgeqwxzs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxuanxn.top/gtbghlphpt.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gtbnwactog.html

memcpy(dst, src, n);
来源：http://hz.xuetiantiany.cn/gtigkyfwjb.html

[S26] C：内存清零
来源：http://hz.jinghuilouyu.cn/gtwnswioar.html

memset(a, 0, sizeof a);
来源：http://hz.zhixingplan.top/gtzoevqspk.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtusurxwmq.html

const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gtfxwynfxb.html

[S28] C：静态变量
来源：http://hz.sweek.top/gteazimuhn.html

static int counter = 0;
来源：http://hz.dashuyun.cn/gtwhhamtgj.html

[S29] C：变参函数
来源：http://hz.zhengqikj.top/gtfyiiilhv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.dianchejie.cn/gtxfdhxdxm.html

[S30] C：头文件保护
来源：http://hz.ydzc1.top/gtafwghmtc.html

#ifndef X_H
来源：http://hz.cqqwz.cn/gtulzrufgm.html

#define X_H
来源：http://hz.jinghuilouyu.cn/gtfopxbsut.html

#endif
来源：http://hz.jqgfzy.top/gtsimlqzbv.html

[S31] C++：Hello World
来源：http://hz.sxryk.cn/gtrdqmcenm.html

#include <iostream>
来源：http://hz.yuxming.cn/gttitrdsef.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtizckoxgh.html

[S32] C++：字符串
来源：http://hz.zhaomingkeji.xyz/gtefkorrwy.html

std::string s = "hi";  s += "!";
来源：http://hz.zycfv.cn/gtkemvnnrg.html

[S33] C++：vector 增删
来源：http://hz.haohaochexian.top/gttokqbaiu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.9152youxi.cn/gtmbtdrepm.html

[S34] C++：遍历 vector
来源：http://hz.nanxuanxn.top/gtscmqgqcn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtcwaelvun.html

[S35] C++：map
来源：http://hz.fengsongda.top/gtrwxrecdu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtnppmlvoe.html

[S36] C++：unordered_map
来源：http://hz.gzhubu.top/gtswqkhnok.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtyaxvjzjz.html

[S37] C++：set
来源：http://hz.fengsongda.top/gtgtcequyv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtyupwiehi.html

[S38] C++：排序
来源：http://hz.hongshengwenyu.top/gttncvqaef.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtiwnthzju.html

[S39] C++：自定义比较器排序
来源：http://hz.birdmap.top/gtttmszbaa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.redwolf501.top/gtpgbydrtc.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtcaxillrn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.feifeiyinyue.top/gtielkpjez.html

[S41] C++：类与构造函数
来源：http://hz.jinqigufen.top/gtvkggmvqq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydjk.org.cn/gtcxdkqobo.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gtkqnekffs.html

class B : public Base { public: void f() override {} };
来源：http://hz.aibaodan.cn/gtxdzezrfp.html

[S43] C++：智能指针
来源：http://hz.zhongyouzk.top/gtkckqjuss.html

auto p = std::make_unique<int>(5);
来源：http://hz.mhx1999.top/gtrtthlyup.html

[S44] C++：引用传参
来源：http://hz.xuetiantiany.cn/gtfkiykjie.html

void inc(int &x) { ++x; }
来源：http://hz.zycfv.cn/gtdgwtwfxu.html

[S45] C++：lambda
来源：http://hz.jinqigufen.top/gtjvxyqtpy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zdqjudy.top/gtytsfiqbg.html

[S46] C++：函数模板
来源：http://hz.daxiang520.top/gtpplnvytq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sysykeji.top/gtfieyrogf.html

[S47] C++：结构化绑定遍历
来源：http://hz.hywenlv.cn/gttmycexvo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guannengcc.top/gtnthcvnvn.html

[S48] C++：逐行读文件
来源：http://hz.wangdashe.top/gtfflvqsza.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.havefunace.top/gtzjnvjunz.html

while (std::getline(in, line)) { }
来源：http://hz.nwbrower.top/gthtlcedxe.html

[S49] C++：写文件
来源：http://hz.feifeiyinyue.top/gthetgbhyv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yonumen.top/gtvpkcaojp.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gtbevdhaef.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jlsjyb.cn/gtltqjtmdu.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtnqdboucu.html

static_cast<double>(a) / b
来源：http://hz.zhaomingkeji.xyz/gticdkxewf.html

[S52] C++：const 与 noexcept
来源：http://hz.ppjwa.cn/gtssykmtaw.html

int size() const noexcept { return n_; }
来源：http://hz.zdqjudy.top/gtypmyxyow.html

[S53] C++：移动语义
来源：http://hz.feifeiyinyue.top/gtfuhwvtih.html

std::vector<int> w = std::move(v);
来源：http://hz.bjfxy.top/gtwmvklgoc.html

[S54] C++：异常处理
来源：http://hz.zdqjudy.top/gtooasslze.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guannengcc.top/gtlpqgxojg.html

[S55] C++：结构化绑定
来源：http://hz.ivvv.top/gtlrmtuqkr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xziqi.cn/gthswhlhug.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtoshvlmjv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnxiangtu.top/gtutukqudr.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtmgdwehbf.html

constexpr int N = 10;
来源：http://hz.yonumen.top/gtcbtfhdpf.html

[S58] C++：命名空间
来源：http://hz.yongpay.top/gtbbzcbplx.html

namespace ns { int f() { return 1; } }
来源：http://hz.yangfankeji.com/gtpoazfsmz.html

[S59] C++：静态断言
来源：http://hz.ivvv.top/gtejzeoylf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.feifeiyinyue.top/gttruuczvt.html

[S60] C++：遍历并删除元素
来源：http://hz.yangfankeji.com/gtmdeckdft.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xuanzx.com/gtzoxnzstx.html

================================================================================
来源：http://hz.ybcxt.top/gtzfdnlofi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtppzfgitc.html

================================================================================
来源：http://hz.svipenyu.cn/gtyubecewl.html

[T01] Kotlin：Hello World
来源：http://hz.xinyue.icu/gtmmmawyqk.html

println("Hello")
来源：http://hz.ybcxt.top/gtaafsfrik.html

[T02] Kotlin：变量
来源：http://hz.feifeiyinyue.top/gtxenzpwwq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.pengpengdd.cyou/gtdbuyhhar.html

[T03] Kotlin：字符串模板
来源：http://hz.yueranfly.top/gtitockmtr.html

"值: $b"
来源：http://hz.sufxvd.cn/gtakfyltqk.html

[T04] Kotlin：空安全
来源：http://hz.pengpengdd.cyou/gtborgvtsv.html

val n: String? = null;  n?.length
来源：http://hz.dianchejie.cn/gtgvfhdyag.html


<!-- 参考信息 -->