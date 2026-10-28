代发 wailian999

set -euo pipefail
来源：http://hz.tian-w.cn/gtppcogvrx.html

[R02] 变量赋值与使用
来源：http://hz.pengpengdd.cyou/gtoyhguuwr.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtpwenkwek.html

[R03] 只读变量
来源：http://hz.ybcxt.top/gtprsgnpqk.html

readonly PI=3.14
来源：http://hz.meibo888.top/gtlpehvlqp.html

[R04] 位置参数
来源：http://hz.yangfankeji.com/gtigpwxdbk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gtzhcamvoz.html

[R05] 参数默认值
来源：http://hz.chenjidiqi.icu/gtezfdvzbu.html

name="${1:-default}"
来源：http://hz.hysaishi.cn/gtrokojuul.html

[R06] 判断命令是否存在
来源：http://hz.zycfv.cn/gtvyyazutc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhaomingkeji.xyz/gteadhnnpb.html

[R07] if 判断文件
来源：http://hz.jinyuanbaomall.cn/gtiswviely.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fzhhl.top/gtmqqobsyf.html

[R08] 数值比较
来源：http://hz.yuxming.cn/gtdmprajfe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhijiandao.cn/gtzmclusuz.html

[R09] 字符串比较
来源：http://hz.xziqi.cn/gtyeqytcqw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yonumen.top/gtudkropfi.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtzhiqzoea.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtgbcwxfwy.html

[R11] case 多分支
来源：http://hz.sxryk.cn/gtdixozwfg.html

case "$1" in
来源：http://hz.hywenlv.cn/gtxkvouato.html

start) echo "启动" ;;
来源：http://hz.yanxiufei.cn/gtockvfudm.html

stop)  echo "停止" ;;
来源：http://hz.hnxiangtu.top/gtnmokqjxq.html

*)     echo "未知命令" ;;
来源：http://hz.hongshengwenyu.top/gtbxddwjlf.html

esac
来源：http://hz.hysaishi.cn/gtujejvxby.html

[R12] for 遍历文件
来源：http://hz.pycfn.com/gtlkajuhno.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cdnleiting.top/gtlorzvtsy.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtyedtaiyx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtidyftnnn.html

[R14] C 风格 for
来源：http://hz.gotoacloud.top/gtiibdjont.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtivtahacv.html

[R15] while 逐行读文件
来源：http://hz.cdnleiting.top/gtvvfqrska.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sxryk.cn/gtreajbmvc.html

[R16] until 等待条件
来源：http://hz.chenzaomai.com/gtestlklyz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtsrnbynag.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gtyvimpgot.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtqztedrhn.html

[R18] 遍历数组
来源：http://hz.cdnleiting.top/gtwuddivqm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ivvv.top/gtnfkajevm.html

[R19] 数组长度
来源：http://hz.zhengqikj.top/gtbggtzjwv.html

echo "${#arr[@]}"
来源：http://hz.zhengqikj.top/gtewdjsovw.html

[R20] 关联数组（字典）
来源：http://hz.daria6918.cn/gtoxgvsfad.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jiagoushi.top/gtongighgb.html

[R21] 字符串长度
来源：http://hz.jlsjyb.cn/gteyqxmwew.html

echo "${#s}"
来源：http://hz.redwolf501.top/gtqtydmhqy.html

[R22] 截取子串
来源：http://hz.yj202588.top/gtnuwswdic.html

echo "${s:0:5}"
来源：http://hz.zhoulong.xyz/gtlsuwzhgt.html

[R23] 字符串替换
来源：http://hz.daxiang520.top/gtdvdkhgxe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yongpay.top/gtgimtxosi.html

[R24] 大小写转换
来源：http://hz.tanke756.top/gtdlytjtfa.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtdskeqpup.html

[R25] 去后缀 / 去前缀
来源：http://hz.jlsjyb.cn/gtufnusrje.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hongshengwenyu.top/gtjarbahda.html

[R26] 命令替换
来源：http://hz.wangdashe.top/gtakrcqzhk.html

now=$(date +%F); echo "$now"
来源：http://hz.jyoumei.cn/gtulxqgvge.html

[R27] 算术展开
来源：http://hz.feifeiyinyue.top/gtxehlfwsu.html

echo $((1 + 2 * 3))
来源：http://hz.pycfn.com/gtuhgchmps.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtpceymuth.html

echo "scale=2; 10/3" | bc
来源：http://hz.snrcjt.cn/gthzaypqlg.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtxosglalb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuxming.cn/gtppvmbenp.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtrcvihlpx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gtzguagzye.html

[R31] 局部变量
来源：http://hz.jinyuanbaomall.cn/gtuekjecjc.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj20258.top/gtfviywaqy.html

[R32] 参数个数校验
来源：http://hz.yj20258.top/gtpxguzrrk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhiwuduotai.top/gthcqqndgl.html

[R33] 捕获错误并提示行号
来源：http://hz.mhx1999.top/gthhuhytxr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxuanxn.top/gtlgwycfre.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gtmsajayia.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtqtmopflx.html

[R35] 后台执行并等待
来源：http://hz.zhongyouzk.top/gtyomnccka.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sufxvd.cn/gtshxtdilf.html

[R36] 并发执行多个任务
来源：http://hz.fengsongda.top/gtjmlppdbb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sysykeji.top/gtqgbeorvp.html

[R37] 把输出赋给变量
来源：http://hz.sxryk.cn/gtzkfmuwbs.html

files=$(ls -1)
来源：http://hz.daria6918.cn/gtayacnbwi.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtbbdfetcl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gzhubu.top/gtcejuulgt.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtinsqphfs.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gtgwgehfto.html

[R40] 追加写日志
来源：http://hz.chenzaomai.com/gtfulwhuxj.html

echo "log" >> out.log
来源：http://hz.xinyue.icu/gtoxpsjrbg.html

[R41] 丢弃输出
来源：http://hz.jlsjyb.cn/gtqbmzxljn.html

cmd >/dev/null 2>&1
来源：http://hz.tanke756.top/gtcxymbtgb.html

[R42] 输入重定向
来源：http://hz.jiagoushi.top/gtaxunoawk.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gttnziwicj.html

[R43] 按名字查找文件
来源：http://hz.gogol.net.cn/gteaemjwpd.html

find . -name "*.log" -type f
来源：http://hz.ppjwa.cn/gtciekzivn.html

[R44] 按修改时间查找
来源：http://hz.ywan-chungtsiang.top/gtkpjzwrlj.html

find . -mtime -7 -type f
来源：http://hz.smart0.xyz/gtmnhszgri.html

[R45] 批量删除
来源：http://hz.xuanzx.com/gtxazhipui.html

find . -name "*.tmp" -delete
来源：http://hz.xuanzx.com/gtyhkrqbfh.html

[R46] 递归替换文件内容
来源：http://hz.cheryme.top/gtqongbiqz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtpodvdasc.html

[R47] sed 单行替换
来源：http://hz.redwolf501.top/gtqknnlemm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hongshengwenyu.top/gttbcxegmo.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gticgtfuyq.html

awk '{print $1, $3}' a.txt
来源：http://hz.cqqwz.cn/gthlqxunhs.html

[R49] awk 带条件
来源：http://hz.meibo888.top/gtgcnkpvrt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.c1oappe.top/gtudfkwhrc.html

[R50] awk 求和
来源：http://hz.feifeiyinyue.top/gtrvstgtkp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xinyue.icu/gttthmsiit.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtznkrsbxe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cdnleiting.top/gtppiduupg.html

[R52] 统计行数
来源：http://hz.shangyingyoupin.top/gteozejltg.html

wc -l a.txt
来源：http://hz.yongpay.top/gtvgjhpsee.html

[R53] 查看文件头与实时尾
来源：http://hz.aizwys.cn/gtlsiiwhzh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jyoumei.cn/gtjldhkfcc.html

[R54] 比较两个文件
来源：http://hz.xuanzx.com/gtpsdevpcb.html

diff a.txt b.txt
来源：http://hz.ivvv.top/gtxnrdvgal.html

[R55] 压缩与解压
来源：http://hz.birdmap.top/gtkevfrvmo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cucudq.cn/gtkyixlgwo.html

[R56] 远程拷贝
来源：http://hz.fengsongda.top/gtqpbggpvt.html

scp file user@host:/path/
来源：http://hz.mhx1999.top/gtpeeopyhz.html

[R57] 远程执行命令
来源：http://hz.meibo888.top/gttehobkri.html

ssh user@host 'uptime'
来源：http://hz.hammf.cn/gtrmccdtqp.html

[R58] 下载文件
来源：http://hz.dianchejie.cn/gtdojtrunh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258.top/gtqnwrpsho.html

[R59] 发 POST JSON
来源：http://hz.xuetiantiany.cn/gtbfnabgtd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.birdmap.top/gtsfaxjrum.html

[R60] 只看 HTTP 状态码
来源：http://hz.zycfv.cn/gtlzarpxpb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenjidiqi.icu/gtzvqqtvqt.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtaryfqmor.html

df -h;  du -sh *
来源：http://hz.aizwys.cn/gtwouhqqqv.html

[R62] 找最占空间的文件
来源：http://hz.aizwys.cn/gtapaznvwp.html

du -ah . | sort -rh | head -10
来源：http://hz.yuanzhike.top/gthfyuqyzf.html

[R63] 内存与进程
来源：http://hz.hnqzz.top/gtqpeguhtc.html

free -h;  ps aux | grep nginx
来源：http://hz.tianlin.xyz/gtojiyxikp.html

[R64] 结束进程
来源：http://hz.kuanghao11.cn/gtmvjnuhvn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tian-w.cn/gtgtzmwwdd.html

[R65] 查看端口占用
来源：http://hz.yj202588.top/gtvgyuggms.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.52xcode.cn/gtviqcqmzp.html

[R66] 定时任务
来源：http://hz.jinqigufen.top/gtbkzewqpk.html

crontab -e;  crontab -l
来源：http://hz.xuetiantiany.cn/gtofodclem.html

[R67] 生成随机十六进制串
来源：http://hz.xuetiantiany.cn/gtasdexmjw.html

openssl rand -hex 16
来源：http://hz.xuanzx.com/gtkyekvthq.html

[R68] 计算文件校验值
来源：http://hz.aibaodan.cn/gtortmlhms.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtjahnqrqa.html

[R69] 生成随机密码
来源：http://hz.ppjwa.cn/gtljndherx.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtttzrivnm.html

[R70] 时间戳与互转
来源：http://hz.zhiwuduotai.top/gtonftmedz.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtmzioabhq.html

[R71] 日期格式化
来源：http://hz.cdnleiting.top/gtpheiacrt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shangyingyoupin.top/gtisdoyleb.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gtofotfvli.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hywenlv.cn/gtbcjjufjs.html

[R73] 分割大日志
来源：http://hz.mhx1999.top/gtjyjmhyxb.html

split -l 1000 big.log part_
来源：http://hz.ehwqpu.com/gtrubqcyfw.html

[R74] 批量重命名
来源：http://hz.xziqi.cn/gtjjmiywzf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtpehgwpnp.html

[R75] 导出环境变量
来源：http://hz.jyoumei.cn/gtyacfcvft.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shzxlz.cn/gtqwbrswbj.html

[R76] 使用临时文件
来源：http://hz.shuidangran.top/gtonbahwvr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtlgwdchoe.html

[R77] 读取用户输入
来源：http://hz.yj20258888.top/gtwmjkmqoc.html

read -rp "请输入: " ans
来源：http://hz.yanxiufei.cn/gtflktwqgq.html

[R78] 交互式菜单
来源：http://hz.ehwqpu.com/gtunskohru.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinghuilouyu.cn/gtdulfovti.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtytcbfhph.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nanxuanxn.top/gtqhldinwb.html

[R80] 查看脚本执行耗时
来源：http://hz.kuanghao11.cn/gtlzedbpra.html

time ./run.sh
来源：http://hz.316326.xyz/gtdcklymnm.html

================================================================================
来源：http://hz.redwolf501.top/gtsxuzmqhs.html

S. C / C++ 专题
来源：http://hz.snrcjt.cn/gttdsodqol.html

================================================================================
来源：http://hz.tanke756.top/gtrrexxoka.html

[S01] C：Hello World
来源：http://hz.aizwys.cn/gtannpbtco.html

#include <stdio.h>
来源：http://hz.ydzc1.top/gtmtzwavod.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuanzhike.top/gtigrhwdfz.html

[S02] C：变量与格式化输出
来源：http://hz.c1oappe.top/gtzktrrxzx.html

int a = 10; printf("%d\n", a);
来源：http://hz.cucudq.cn/gtmwdqfyij.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gthclffudh.html

int x; scanf("%d", &x);
来源：http://hz.snrcjt.cn/gtvfrnhbcp.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gtdcsrilli.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jyoumei.cn/gtpvylxqrx.html

[S05] C：字符串长度
来源：http://hz.shzxlz.cn/gthwjcmqod.html

strlen(s)
来源：http://hz.hnxiangtu.top/gtrpkrvoaa.html

[S06] C：字符串比较
来源：http://hz.shangyingyoupin.top/gtsbatiucm.html

strcmp(a, b) == 0
来源：http://hz.nanxuanxn.top/gthikzrykk.html

[S07] C：数组遍历求和
来源：http://hz.bjfxy.top/gttuxxgtuh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.svipenyu.cn/gtautqbtok.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258888.top/gtbyxnqptu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.9152youxi.cn/gtymaasvnj.html

[S09] C：结构体定义与初始化
来源：http://hz.gotoacloud.top/gtdkqzfnvs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnqzz.top/gtzhompixz.html

[S10] C：指针与解引用
来源：http://hz.nanxinkj.top/gtzmmiqwdt.html

int *p = &a;  *p = 5;
来源：http://hz.fengsongda.top/gtoymcapfb.html

[S11] C：逐行读文件
来源：http://hz.kuanghao11.cn/gtzsjmsvil.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xinyue.icu/gtwnspvqio.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuanzhike.top/gtmbgkmkpu.html

fclose(f);
来源：http://hz.bjfxy.top/gtceilmgwu.html

[S12] C：写文件
来源：http://hz.tanke756.top/gtguhfilnq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.bjfxy.top/gtuprnfuhj.html

[S13] C：宏定义
来源：http://hz.ehwqpu.com/gtnooyrtad.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhixingplan.top/gtsdsfjovy.html

[S14] C：枚举
来源：http://hz.wangshuangyany.cn/gtibicwneu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.iojbl.cn/gthtizvdqn.html

[S15] C：类型转换
来源：http://hz.yangfankeji.com/gtnluhqapj.html

(double) a / b
来源：http://hz.feifeiyinyue.top/gtybeybilz.html

[S16] C：位操作置位
来源：http://hz.yuxming.cn/gtwlddfqgj.html

x |= (1 << 3);
来源：http://hz.jinqigfzy.top/gtvjlrkzgk.html

[S17] C：安全拼接字符串
来源：http://hz.pycfn.com/gtksnikjzh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yvedp.cn/gtdbzxkkil.html

[S18] C：命令行参数
来源：http://hz.ppjwa.cn/gttkgoltdh.html

int main(int argc, char **argv)
来源：http://hz.shuidangran.top/gtmocgxger.html

[S19] C：快速排序
来源：http://hz.ybcxt.top/gtjvefuhnz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtnqzmanyb.html

[S20] C：二分查找
来源：http://hz.redwolf501.top/gtzeaotmco.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtnnqqdsvq.html

[S21] C：字符类别判断
来源：http://hz.shangyingyoupin.top/gtnzdproyr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hnxiangtu.top/gtibergwqk.html

[S22] C：字符串转数字
来源：http://hz.yuxming.cn/gtlaudqwbk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuanzhike.top/gtwgkfwoeo.html

[S23] C：随机数
来源：http://hz.svipenyu.cn/gteqludrge.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj20258.top/gtelppikru.html

[S24] C：获取本地时间
来源：http://hz.xylfe.cn/gtofwseesv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fengsongda.top/gtzolcfngv.html

[S25] C：内存拷贝
来源：http://hz.zhongyouzk.top/gtajmouyzn.html

memcpy(dst, src, n);
来源：http://hz.svipenyu.cn/gttoncutqe.html

[S26] C：内存清零
来源：http://hz.zhiwuduotai.top/gtcdclhlvn.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtvuxqknjd.html

[S27] C：定义常量
来源：http://hz.sysykeji.top/gtlbrztieb.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtpvzuhboi.html

[S28] C：静态变量
来源：http://hz.jiagoushi.top/gthbqnsmbj.html

static int counter = 0;
来源：http://hz.chenzaomai.com/gttypulpey.html

[S29] C：变参函数
来源：http://hz.zhiwuduotai.top/gtljtabosc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhaomingkeji.xyz/gtcyiqmdti.html

[S30] C：头文件保护
来源：http://hz.zycfv.cn/gtysgejybn.html

#ifndef X_H
来源：http://hz.hnxiangtu.top/gtkyaozvsw.html

#define X_H
来源：http://hz.chenlongwang.top/gtasuxgquj.html

#endif
来源：http://hz.zhoulong.xyz/gtihzrcgdm.html

[S31] C++：Hello World
来源：http://hz.guannengcc.top/gthucmxbvs.html

#include <iostream>
来源：http://hz.zhengqikj.top/gttbxagutd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangkeji.top/gtysisttdt.html

[S32] C++：字符串
来源：http://hz.smart0.xyz/gtsgoohnxr.html

std::string s = "hi";  s += "!";
来源：http://hz.xingfuxueyuan.xyz/gtnicfdkjq.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtmixmtcfd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hnqzz.top/gtjootdago.html

[S34] C++：遍历 vector
来源：http://hz.nwbrower.top/gtkjrszvhb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cheryme.top/gtwoitybbw.html

[S35] C++：map
来源：http://hz.ywan-chungtsiang.top/gtsufsrxjy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guowangkeji.top/gtaqagogvb.html

[S36] C++：unordered_map
来源：http://hz.yuxming.cn/gtixnmfxia.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtsliqnkad.html

[S37] C++：set
来源：http://hz.daxiang520.top/gtvnnkmclx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj202588.top/gtgrvdonrw.html

[S38] C++：排序
来源：http://hz.nanxuanxn.top/gtbmjijapu.html

std::sort(v.begin(), v.end());
来源：http://hz.ehwqpu.com/gtyvlyxbus.html

[S39] C++：自定义比较器排序
来源：http://hz.jianghu66.top/gtcixoxblb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hywenlv.cn/gtbfceudgj.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gtrrduhlih.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shzxlz.cn/gtaogtnyrd.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtwdpdereo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yangfankeji.com/gtxubokuxo.html

[S42] C++：继承与虚函数
来源：http://hz.yanxiufei.cn/gtvmtyhhuk.html

class B : public Base { public: void f() override {} };
来源：http://hz.jiagoushi.top/gtkafkazeh.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtnxpjgoqq.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtqydglwzy.html

[S44] C++：引用传参
来源：http://hz.aizwys.cn/gtoosxpayz.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gtxnyxsdpu.html

[S45] C++：lambda
来源：http://hz.cheryme.top/gttbzbcdfg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhengqikj.top/gtozniqyst.html

[S46] C++：函数模板
来源：http://hz.xylfe.cn/gtsyufwxsk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xingfuxueyuan.xyz/gtldqeacdb.html

[S47] C++：结构化绑定遍历
来源：http://hz.yongpay.top/gtvsqjgnpe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jyoumei.cn/gttlmrtmkd.html

[S48] C++：逐行读文件
来源：http://hz.hysaishi.cn/gtxerjkchv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtriourgkp.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtxokdrewb.html

[S49] C++：写文件
来源：http://hz.redwolf501.top/gtedllnkel.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.andypj.xyz/gtiqwidulf.html

[S50] C++：格式化数字
来源：http://hz.shangyingyoupin.top/gtnmcylfjv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yueranfly.top/gtotqpartq.html

[S51] C++：显式类型转换
来源：http://hz.svipenyu.cn/gtsxsvzorc.html

static_cast<double>(a) / b
来源：http://hz.jqgfzy.top/gtcywafckc.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtbqfkkyxn.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtnsqtxouf.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gtttxthujy.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtxplqbqvh.html

[S54] C++：异常处理
来源：http://hz.yueranfly.top/gtavaalgkr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gotoacloud.top/gtzdlsayze.html

[S55] C++：结构化绑定
来源：http://hz.9152youxi.cn/gthkaleupa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dianchejie.cn/gtxjxssuqp.html

[S56] C++：optional
来源：http://hz.chenjidiqi.icu/gthbnkpqop.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ywan-chungtsiang.top/gtiusjheza.html

[S57] C++：编译期常量
来源：http://hz.zhijiandao.cn/gtlduvqxtt.html

constexpr int N = 10;
来源：http://hz.hfpthk.cn/gtstdnexyh.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gtosoacsaa.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenlongwang.top/gtyesbwvkf.html

[S59] C++：静态断言
来源：http://hz.yvedp.cn/gtfjjvffii.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.0kj1m.cn/gtqedncphn.html

[S60] C++：遍历并删除元素
来源：http://hz.xziqi.cn/gthdecfegi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tanke756.top/gthtrwuhmt.html

================================================================================
来源：http://hz.vqdsnc.cn/gtffydxeaf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuanzhike.top/gtewkjdesb.html

================================================================================
来源：http://hz.sweek.top/gtzzdslldm.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gtxmewabrh.html

println("Hello")
来源：http://hz.tian-w.cn/gtnlmnequy.html

[T02] Kotlin：变量
来源：http://hz.sweek.top/gtlzuxrcyj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuxming.cn/gtroxgtuvg.html


<!-- 参考信息 -->