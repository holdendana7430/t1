代发 wailian999

name="${1:-default}"
来源：http://hz.jqgfzy.top/gtymdbdhhl.html

[R06] 判断命令是否存在
来源：http://hz.sweek.top/gtvjzzcmpd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgufenzy.top/gtvajvkkhb.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtrlnmmpxd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guowangkeji.top/gtkqnnoydk.html

[R08] 数值比较
来源：http://hz.gaohongyu789.top/gtubswfnob.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gthcbzaxuu.html

[R09] 字符串比较
来源：http://hz.shuidangran.top/gtstnyzrrm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xinyue.icu/gtyxfmlsbr.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtlaytbapi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.smart0.xyz/gtlwfexryt.html

[R11] case 多分支
来源：http://hz.ehwqpu.com/gtfdkezmfm.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gtmizjwqgd.html

start) echo "启动" ;;
来源：http://hz.sweek.top/gtauvwqthy.html

stop)  echo "停止" ;;
来源：http://hz.yonumen.top/gtcaapbolc.html

*)     echo "未知命令" ;;
来源：http://hz.yvedp.cn/gtatxueazx.html

esac
来源：http://hz.yangfankeji.com/gtvidassvm.html

[R12] for 遍历文件
来源：http://hz.hongshengwenyu.top/gtctjpqych.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtwfeibohq.html

[R13] for 计数循环
来源：http://hz.yonumen.top/gtyovmlecf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pycfn.com/gtbqetwknd.html

[R14] C 风格 for
来源：http://hz.pycfn.com/gtnbhedyqn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtvnvwlqua.html

[R15] while 逐行读文件
来源：http://hz.jianghu66.top/gtalfrzfnz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.52xcode.cn/gtmviygxyn.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gtjznxumro.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtolslhhah.html

[R17] 数组定义与取值
来源：http://hz.xuetiantiany.cn/gtznixbpba.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.snrcjt.cn/gtyqgyogbr.html

[R18] 遍历数组
来源：http://hz.aibaodan.cn/gtsckftmxw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtzyelvkxy.html

[R19] 数组长度
来源：http://hz.daxiang520.top/gtzemkzuzh.html

echo "${#arr[@]}"
来源：http://hz.havefunace.top/gtijzvbwgw.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtbmlkbvyq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.pycfn.com/gtlefvcxcp.html

[R21] 字符串长度
来源：http://hz.hywenlv.cn/gtpwvgpjxz.html

echo "${#s}"
来源：http://hz.shuidangran.top/gtxpvvhxgv.html

[R22] 截取子串
来源：http://hz.shanyushiyangkeji.top/gtetvekfnv.html

echo "${s:0:5}"
来源：http://hz.hywenlv.cn/gtcatzuoem.html

[R23] 字符串替换
来源：http://hz.yangfankeji.com/gtkpamusoj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinyuanbaomall.cn/gtjuvhidwg.html

[R24] 大小写转换
来源：http://hz.wangshuangyany.cn/gtotlnufqq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daria6918.cn/gtrziogxio.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtpwkcizzf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gttoygiwth.html

[R26] 命令替换
来源：http://hz.xylfe.cn/gttjcsfhyz.html

now=$(date +%F); echo "$now"
来源：http://hz.guannengcc.top/gtdxlmctsa.html

[R27] 算术展开
来源：http://hz.ivvv.top/gtpautvpoh.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtwnwkxafq.html

[R28] 浮点运算
来源：http://hz.jinyuanbaomall.cn/gtcaxyuwfo.html

echo "scale=2; 10/3" | bc
来源：http://hz.sysykeji.top/gtngqlvfca.html

[R29] 定义函数
来源：http://hz.gaohongyu789.top/gtgnsbxvmf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gtowdzixoc.html

[R30] 函数返回状态码
来源：http://hz.smart0.xyz/gtburhulnu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jlsjyb.cn/gtfjiguqul.html

[R31] 局部变量
来源：http://hz.jianghu66.top/gtynumdqyz.html

f() { local x=1; echo "$x"; }
来源：http://hz.jiagoushi.top/gtyaaitfgm.html

[R32] 参数个数校验
来源：http://hz.ivvv.top/gtbbdipbny.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuanzx.com/gtxurtyehb.html

[R33] 捕获错误并提示行号
来源：http://hz.daxiang520.top/gttorsikoe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gaohongyu789.top/gttcrgqwoq.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gtiuanwpjn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtimnevnau.html

[R35] 后台执行并等待
来源：http://hz.tanke756.top/gtuvghsbfl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtiwdnrqsb.html

[R36] 并发执行多个任务
来源：http://hz.nwbrower.top/gtoynjfnkd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ehwqpu.com/gtwohfuguk.html

[R37] 把输出赋给变量
来源：http://hz.birdmap.top/gtwozlcsoe.html

files=$(ls -1)
来源：http://hz.316326.xyz/gtdyzmgxta.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtglcqaggi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daria6918.cn/gtobvvdpid.html

[R39] 重定向标准输出与错误
来源：http://hz.gogol.net.cn/gtbumuidtx.html

cmd > out.log 2>&1
来源：http://hz.yongpay.top/gtjxpbbroz.html

[R40] 追加写日志
来源：http://hz.52xcode.cn/gtyurbihac.html

echo "log" >> out.log
来源：http://hz.shanyushiyangkeji.top/gtsijzshsa.html

[R41] 丢弃输出
来源：http://hz.dashuyun.cn/gtpcenkowr.html

cmd >/dev/null 2>&1
来源：http://hz.shuidangran.top/gtytnoklll.html

[R42] 输入重定向
来源：http://hz.52xcode.cn/gttssqyfwg.html

wc -l < a.txt
来源：http://hz.ywan-chungtsiang.top/gtqnashodd.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtupfzcewv.html

find . -name "*.log" -type f
来源：http://hz.yuxming.cn/gtmgoppycc.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtzliyrfig.html

find . -mtime -7 -type f
来源：http://hz.nanxinkj.top/gtjgxtudtf.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gtfzmzucpm.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigufen.top/gtqgjqscnc.html

[R46] 递归替换文件内容
来源：http://hz.yanxiufei.cn/gtymbnxroi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtkvidvtve.html

[R47] sed 单行替换
来源：http://hz.shangyingyoupin.top/gtirunahkw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gtiodjsmog.html

[R48] awk 取指定列
来源：http://hz.jqgufenzy.top/gtafnzjmsq.html

awk '{print $1, $3}' a.txt
来源：http://hz.hywenlv.cn/gtbduuvqpp.html

[R49] awk 带条件
来源：http://hz.yj20258.top/gtkecrnsbc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.0kj1m.cn/gtoeufelfz.html

[R50] awk 求和
来源：http://hz.aibaodan.cn/gtpmcmvgvr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xylfe.cn/gtjctmvbqt.html

[R51] 排序去重取前几
来源：http://hz.ehwqpu.com/gtpxcmvljm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.andypj.xyz/gtuoqlrpla.html

[R52] 统计行数
来源：http://hz.xingfuxueyuan.xyz/gtlplxtyuk.html

wc -l a.txt
来源：http://hz.ybcxt.top/gtsikycuxx.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gtkatfspfh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtnsygtzrk.html

[R54] 比较两个文件
来源：http://hz.ivvv.top/gtvfvazwfe.html

diff a.txt b.txt
来源：http://hz.svipenyu.cn/gtqujjndqz.html

[R55] 压缩与解压
来源：http://hz.zdqjudy.top/gtbuhjrizu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtpfqttari.html

[R56] 远程拷贝
来源：http://hz.snrcjt.cn/gtuiumsotc.html

scp file user@host:/path/
来源：http://hz.bjfxy.top/gtongdgysm.html

[R57] 远程执行命令
来源：http://hz.chenlongwang.top/gtmmthugnt.html

ssh user@host 'uptime'
来源：http://hz.jlsjyb.cn/gtsfnoxzcm.html

[R58] 下载文件
来源：http://hz.9152youxi.cn/gtkkkuvboq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gtboehqxib.html

[R59] 发 POST JSON
来源：http://hz.sufxvd.cn/gtdoujofmu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtgyxbiqrv.html

[R60] 只看 HTTP 状态码
来源：http://hz.sysykeji.top/gtxshbhead.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.9152youxi.cn/gtdudbrfjm.html

[R61] 磁盘占用
来源：http://hz.meibo888.top/gtdujglhap.html

df -h;  du -sh *
来源：http://hz.jianghu66.top/gtcgbxnczg.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtjjclycxf.html

du -ah . | sort -rh | head -10
来源：http://hz.hfpthk.cn/gtxwejgzsd.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtokvmmuan.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gttrptmrfk.html

[R64] 结束进程
来源：http://hz.smart0.xyz/gthxcwcakj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.andypj.xyz/gthpuodrln.html

[R65] 查看端口占用
来源：http://hz.zdqjudy.top/gtmccvcsqh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.meibo888.top/gtdxucghck.html

[R66] 定时任务
来源：http://hz.yanxiufei.cn/gtwzcrzvvl.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtifyomybc.html

[R67] 生成随机十六进制串
来源：http://hz.zhoulong.xyz/gtdsxhrlkl.html

openssl rand -hex 16
来源：http://hz.havefunace.top/gthyuytoun.html

[R68] 计算文件校验值
来源：http://hz.birdmap.top/gtwzznmwup.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtebegiytd.html

[R69] 生成随机密码
来源：http://hz.nwbrower.top/gtpszxnyjt.html

head -c 16 /dev/urandom | base64
来源：http://hz.tanke756.top/gtqwsewlwl.html

[R70] 时间戳与互转
来源：http://hz.yj20258.top/gtqghtclhw.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtozbtpzjm.html

[R71] 日期格式化
来源：http://hz.nanxinkj.top/gtawuvfgda.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ywan-chungtsiang.top/gtzdxcalln.html

[R72] 等待端口就绪
来源：http://hz.c1oappe.top/gtflvbmomq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtfjwwcwds.html

[R73] 分割大日志
来源：http://hz.jlsjyb.cn/gthorzdfqh.html

split -l 1000 big.log part_
来源：http://hz.zhongyouzk.top/gttzylnshp.html

[R74] 批量重命名
来源：http://hz.redwolf501.top/gtguikklwb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.316326.xyz/gtpznokxws.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtwuldzizj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtdtjnuffm.html

[R76] 使用临时文件
来源：http://hz.hnqzz.top/gtuwpnqwod.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtsgwserxm.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtyqmcddwo.html

read -rp "请输入: " ans
来源：http://hz.zdqjudy.top/gtbktmgsga.html

[R78] 交互式菜单
来源：http://hz.ehwqpu.com/gtxulznxfr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.birdmap.top/gtpiryomkh.html

[R79] 解析命令行选项
来源：http://hz.ywan-chungtsiang.top/gtrefiktkb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.meibo888.top/gtuvuctgoh.html

[R80] 查看脚本执行耗时
来源：http://hz.havefunace.top/gtsnbeuvwh.html

time ./run.sh
来源：http://hz.yj202588.top/gtoquoeola.html

================================================================================
来源：http://hz.shzxlz.cn/gtppffkxod.html

S. C / C++ 专题
来源：http://hz.redwolf501.top/gtqrczhnsr.html

================================================================================
来源：http://hz.52xcode.cn/gttkeayizo.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtvqwswfbn.html

#include <stdio.h>
来源：http://hz.yanxiufei.cn/gtwtnmvupa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jianghu66.top/gtkvdyinpi.html

[S02] C：变量与格式化输出
来源：http://hz.shzxlz.cn/gtbaryiwsn.html

int a = 10; printf("%d\n", a);
来源：http://hz.havefunace.top/gtgwiavzly.html

[S03] C：读入整数
来源：http://hz.yuxming.cn/gtjrslgzye.html

int x; scanf("%d", &x);
来源：http://hz.smart0.xyz/gtharrbatn.html

[S04] C：字符串复制
来源：http://hz.zdqjudy.top/gthiujlbwe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtqssdypzk.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtkyzpthmm.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtmjiyxdfo.html

[S06] C：字符串比较
来源：http://hz.xinyue.icu/gtpbxgrrsu.html

strcmp(a, b) == 0
来源：http://hz.hywenlv.cn/gtkqgatzuh.html

[S07] C：数组遍历求和
来源：http://hz.yuxming.cn/gtzgoxwtwl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hysaishi.cn/gtrjenxpzk.html

[S08] C：动态内存分配与释放
来源：http://hz.hongshengwenyu.top/gtxoqpareb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hywenlv.cn/gtnngysebl.html

[S09] C：结构体定义与初始化
来源：http://hz.yvedp.cn/gtxeohsmub.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuanzx.com/gtkjzyncbr.html

[S10] C：指针与解引用
来源：http://hz.zdqjudy.top/gtxaxhxfak.html

int *p = &a;  *p = 5;
来源：http://hz.zhixingplan.top/gtthcsvace.html

[S11] C：逐行读文件
来源：http://hz.quarkkingdee.top/gtchpillef.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.kuanghao11.cn/gtzdwxepff.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnqzz.top/gtwiacumvy.html

fclose(f);
来源：http://hz.aibaodan.cn/gtzqqilpaj.html

[S12] C：写文件
来源：http://hz.ydzc1.top/gtolncgswv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangdashe.top/gtsduralxa.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gtapkyvgja.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yongpay.top/gtyvsaeiyo.html

[S14] C：枚举
来源：http://hz.zhiwuduotai.top/gtegluptff.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.svipenyu.cn/gtgkzcshqv.html

[S15] C：类型转换
来源：http://hz.zhiwuduotai.top/gtrbdacoav.html

(double) a / b
来源：http://hz.snrcjt.cn/gtzaixzykp.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtmgproqeq.html

x |= (1 << 3);
来源：http://hz.yuanzhike.top/gtqmzqwbdj.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtmctnyisu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.52xcode.cn/gtoagusrnu.html

[S18] C：命令行参数
来源：http://hz.zhoulong.xyz/gttxnmbgls.html

int main(int argc, char **argv)
来源：http://hz.tanke756.top/gtvpqbsdnm.html

[S19] C：快速排序
来源：http://hz.0kj1m.cn/gtivrappar.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.wangshuangyany.cn/gtrowzivve.html

[S20] C：二分查找
来源：http://hz.zhiwuduotai.top/gtpsirhxrb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuetiantiany.cn/gtlmelcarm.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtoxkgcgfi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.havefunace.top/gtfahtludv.html

[S22] C：字符串转数字
来源：http://hz.hysaishi.cn/gtclnxqloj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dashuyun.cn/gteroodvlp.html

[S23] C：随机数
来源：http://hz.nanxuanxn.top/gtjzhamujx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sweek.top/gtxoddjwbk.html

[S24] C：获取本地时间
来源：http://hz.wangdashe.top/gtufmdothw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hywenlv.cn/gtdhlrszky.html

[S25] C：内存拷贝
来源：http://hz.jiagoushi.top/gtcbwhpkqz.html

memcpy(dst, src, n);
来源：http://hz.sysykeji.top/gtrbeoklcv.html

[S26] C：内存清零
来源：http://hz.xylfe.cn/gtqjdazojm.html

memset(a, 0, sizeof a);
来源：http://hz.jinyuanbaomall.cn/gtxuiddaiq.html

[S27] C：定义常量
来源：http://hz.xylfe.cn/gtyzacxtdf.html

const double PI = 3.14159;
来源：http://hz.cashguo.top/gtjlyopvmo.html

[S28] C：静态变量
来源：http://hz.chenjidiqi.icu/gtfqflilzk.html

static int counter = 0;
来源：http://hz.cdnleiting.top/gtjiyyvueb.html

[S29] C：变参函数
来源：http://hz.jinghuilouyu.cn/gtxlhhblrd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigfzy.top/gtknhczlox.html

[S30] C：头文件保护
来源：http://hz.ywan-chungtsiang.top/gtirkhzvda.html

#ifndef X_H
来源：http://hz.hywenlv.cn/gtxiwvyffc.html

#define X_H
来源：http://hz.xuetiantiany.cn/gtdbjeyosq.html

#endif
来源：http://hz.redwolf501.top/gtqsxxiucq.html

[S31] C++：Hello World
来源：http://hz.kuanghao11.cn/gtfkufmcgn.html

#include <iostream>
来源：http://hz.chenlongwang.top/gtrmpcemup.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hfpthk.cn/gtsmkfkuoi.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtayhppajj.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtukmosiif.html

[S33] C++：vector 增删
来源：http://hz.aibaodan.cn/gtzlcwbgwq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangtech.top/gtqlpfvqwp.html

[S34] C++：遍历 vector
来源：http://hz.ydjk.org.cn/gtpcghlmsh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.aizwys.cn/gtgtqstonq.html

[S35] C++：map
来源：http://hz.gogol.net.cn/gtmzcpxgko.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtegczilop.html

[S36] C++：unordered_map
来源：http://hz.daria6918.cn/gtbjgaatug.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtedwvhjsn.html

[S37] C++：set
来源：http://hz.ivvv.top/gtcnbqdfnp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tanke756.top/gtunpwjazq.html

[S38] C++：排序
来源：http://hz.ybcxt.top/gtffmfuhqo.html

std::sort(v.begin(), v.end());
来源：http://hz.cheryme.top/gttttaafgd.html

[S39] C++：自定义比较器排序
来源：http://hz.hnqzz.top/gtxgdiyecx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtqkadjgcr.html

[S40] C++：查找元素
来源：http://hz.zhiwuduotai.top/gtypfdrlql.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.quarkkingdee.top/gtqhqiymtg.html

[S41] C++：类与构造函数
来源：http://hz.chenjidiqi.icu/gtnvmxvhzx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.redwolf501.top/gtjppqvsrt.html

[S42] C++：继承与虚函数
来源：http://hz.zycfv.cn/gtrxupsnma.html

class B : public Base { public: void f() override {} };
来源：http://hz.sufxvd.cn/gtrcqesrbm.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gtaynvjhts.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgfzy.top/gtkmveptlg.html

[S44] C++：引用传参
来源：http://hz.xuanzx.com/gtzvucbyjb.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangtech.top/gtrosjjdih.html

[S45] C++：lambda
来源：http://hz.shuidangran.top/gtkosueicq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hnxiangtu.top/gtjtewjgtl.html

[S46] C++：函数模板
来源：http://hz.bjfxy.top/gtrcmbmnoc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xinyue.icu/gtzepbljpi.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuanzhike.top/gtclwpqnww.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhongyouzk.top/gtlelrbkzu.html

[S48] C++：逐行读文件
来源：http://hz.jqgfzy.top/gtbdkqycrp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.meibo888.top/gttghqbnmy.html

while (std::getline(in, line)) { }
来源：http://hz.zhixingplan.top/gtbtfemegj.html

[S49] C++：写文件
来源：http://hz.gotoacloud.top/gtquqdcosw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuanzhike.top/gtxhbrhmbs.html

[S50] C++：格式化数字
来源：http://hz.jinqigufen.top/gtddgjteid.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtyhypyvwx.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtxbmrgzsu.html

static_cast<double>(a) / b
来源：http://hz.ehwqpu.com/gticgyjxmw.html

[S52] C++：const 与 noexcept
来源：http://hz.cqqwz.cn/gthbwfzwvt.html

int size() const noexcept { return n_; }
来源：http://hz.ehwqpu.com/gtjpewxnho.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtjlmiekjq.html

std::vector<int> w = std::move(v);
来源：http://hz.jiagoushi.top/gtuhkzwpdh.html

[S54] C++：异常处理
来源：http://hz.hywenlv.cn/gtxqkoekrp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtfyohqiyy.html

[S55] C++：结构化绑定
来源：http://hz.zhoulong.xyz/gtgcpzuaph.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtydywsxai.html

[S56] C++：optional
来源：http://hz.gotoacloud.top/gtlegxsmxw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cashguo.top/gtxaeokjjl.html

[S57] C++：编译期常量
来源：http://hz.yj20258.top/gtzdggiail.html

constexpr int N = 10;
来源：http://hz.vqdsnc.cn/gtzpuqcmuc.html

[S58] C++：命名空间
来源：http://hz.jinqigfzy.top/gtsvcdvegb.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtzpfkoorf.html

[S59] C++：静态断言
来源：http://hz.hywenlv.cn/gtkfveypzv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daria6918.cn/gtmaeuzuob.html

[S60] C++：遍历并删除元素
来源：http://hz.sysykeji.top/gtymdsasbs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgufenzy.top/gtphboeibh.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxfiimfmo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangshuangyany.cn/gtgrimagqh.html

================================================================================
来源：http://hz.c1oappe.top/gtwvimrmkw.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtvrbcimno.html

println("Hello")
来源：http://hz.jqgufenzy.top/gtgjvnzlih.html

[T02] Kotlin：变量
来源：http://hz.zhaomingkeji.xyz/gtumkoipqp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.c1oappe.top/gtwjamnnvu.html

[T03] Kotlin：字符串模板
来源：http://hz.cucudq.cn/gtswxgxvqo.html

"值: $b"
来源：http://hz.yueranfly.top/gtvfbzcclc.html

[T04] Kotlin：空安全
来源：http://hz.ydjk.org.cn/gtziqafcji.html

val n: String? = null;  n?.length
来源：http://hz.guowangkeji.top/gtocduutby.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigufen.top/gtkcmxxifp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cqqwz.cn/gtjqcyngvp.html

[T06] Kotlin：集合映射
来源：http://hz.ywan-chungtsiang.top/gtvakivobn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtquewjuhm.html


<!-- 参考信息 -->