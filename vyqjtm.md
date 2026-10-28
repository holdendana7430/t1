代发 wailian999

set -euo pipefail
来源：http://hz.tanke756.top/gteggajxfu.html

[R02] 变量赋值与使用
来源：http://hz.aibaodan.cn/gtxbdjxvir.html

name="Tom"; echo "$name"
来源：http://hz.chenlongwang.top/gtyflsdmjg.html

[R03] 只读变量
来源：http://hz.pycfn.com/gtqymozkod.html

readonly PI=3.14
来源：http://hz.tanke756.top/gtgpfnuwre.html

[R04] 位置参数
来源：http://hz.gzhubu.top/gtxnfhqbjs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hfpthk.cn/gtmiahfxkb.html

[R05] 参数默认值
来源：http://hz.quarkkingdee.top/gtpoehxdio.html

name="${1:-default}"
来源：http://hz.quarkkingdee.top/gtzeubusim.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtctgzbyny.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cdnleiting.top/gtifdhsgnp.html

[R07] if 判断文件
来源：http://hz.kuanghao11.cn/gtmhvayimo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhiwuduotai.top/gtuhurzkqp.html

[R08] 数值比较
来源：http://hz.sysykeji.top/gtwbivarom.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenzaomai.com/gtzpmufugy.html

[R09] 字符串比较
来源：http://hz.shangyingyoupin.top/gtzcmjlrxs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtlvfjhnzd.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtudxjahnc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtikgyoyox.html

[R11] case 多分支
来源：http://hz.xingfuxueyuan.xyz/gtoutcbmbj.html

case "$1" in
来源：http://hz.daxiang520.top/gttfefaorf.html

start) echo "启动" ;;
来源：http://hz.jlsjyb.cn/gttpzipyfk.html

stop)  echo "停止" ;;
来源：http://hz.wangshuangyany.cn/gtiqsakahg.html

*)     echo "未知命令" ;;
来源：http://hz.zdqjudy.top/gtsbtnsmvj.html

esac
来源：http://hz.tian-w.cn/gtaokaujvg.html

[R12] for 遍历文件
来源：http://hz.zycfv.cn/gtsiemgwln.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtytpbhtod.html

[R13] for 计数循环
来源：http://hz.hnxiangtu.top/gtvuizqdvy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nwbrower.top/gthdnwfjxc.html

[R14] C 风格 for
来源：http://hz.yueranfly.top/gtpunfprmp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxinkj.top/gtbhvkwimn.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gtssnepbiq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.vqdsnc.cn/gtvnmhewgc.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gttyamylgf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtsvlijtbq.html

[R17] 数组定义与取值
来源：http://hz.pengpengdd.cyou/gtoosucpbn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hongshengwenyu.top/gtgokherpe.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gtngsgelvy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zycfv.cn/gtqnnwtalc.html

[R19] 数组长度
来源：http://hz.daxiang520.top/gtofukbreg.html

echo "${#arr[@]}"
来源：http://hz.sufxvd.cn/gtgqoenwdy.html

[R20] 关联数组（字典）
来源：http://hz.yuxming.cn/gtkvdwuvji.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hammf.cn/gtjgkmiouf.html

[R21] 字符串长度
来源：http://hz.jqgfzy.top/gtrprvkqzb.html

echo "${#s}"
来源：http://hz.wangshuangyany.cn/gtgwzoehfh.html

[R22] 截取子串
来源：http://hz.chenzaomai.com/gtupobbxsc.html

echo "${s:0:5}"
来源：http://hz.quarkkingdee.top/gtqiwahubw.html

[R23] 字符串替换
来源：http://hz.bjfxy.top/gtsfvvqyxy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tanke756.top/gtfyzkusxd.html

[R24] 大小写转换
来源：http://hz.tianlin.xyz/gtofqvxrwj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gaohongyu789.top/gtupynyqtf.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuetiantiany.cn/gtikolzttn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sufxvd.cn/gtkjpqzslh.html

[R26] 命令替换
来源：http://hz.aibaodan.cn/gtsueegdot.html

now=$(date +%F); echo "$now"
来源：http://hz.cucudq.cn/gtzoemrrtc.html

[R27] 算术展开
来源：http://hz.yj20258888.top/gtpmuerrpn.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtcrlmpake.html

[R28] 浮点运算
来源：http://hz.chenzaomai.com/gtzxpbybmf.html

echo "scale=2; 10/3" | bc
来源：http://hz.hysaishi.cn/gtugirqhhg.html

[R29] 定义函数
来源：http://hz.jianghu66.top/gtspsaonxg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhengqikj.top/gtlqmfqeut.html

[R30] 函数返回状态码
来源：http://hz.cdnleiting.top/gtedntibto.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nwbrower.top/gtzhkjidux.html

[R31] 局部变量
来源：http://hz.shanyushiyangkeji.top/gtoomrhgqx.html

f() { local x=1; echo "$x"; }
来源：http://hz.shangyingyoupin.top/gtfpoiksaj.html

[R32] 参数个数校验
来源：http://hz.xuetiantiany.cn/gtfzyraoun.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtyeihpcym.html

[R33] 捕获错误并提示行号
来源：http://hz.fzhhl.top/gtbkmcpvfv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ybcxt.top/gtxdscmgxb.html

[R34] 退出时清理
来源：http://hz.zhiwuduotai.top/gtnlksmznr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtkpnwbxdv.html

[R35] 后台执行并等待
来源：http://hz.ydzc1.top/gtjeecfyrw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ehwqpu.com/gthmjovdrs.html

[R36] 并发执行多个任务
来源：http://hz.zhoulong.xyz/gtjroyrthh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.snrcjt.cn/gtlstnatwm.html

[R37] 把输出赋给变量
来源：http://hz.zhijiandao.cn/gtvoehnozx.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtwustfstj.html

[R38] 管道串联
来源：http://hz.wangshuangyany.cn/gthxkyjgih.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tanke756.top/gttdhlvkii.html

[R39] 重定向标准输出与错误
来源：http://hz.guannengcc.top/gtknkckgyb.html

cmd > out.log 2>&1
来源：http://hz.wangdashe.top/gtvzodyejb.html

[R40] 追加写日志
来源：http://hz.zhengqikj.top/gtzvxdgxou.html

echo "log" >> out.log
来源：http://hz.smart0.xyz/gtwrarghow.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gtoxtzpqcz.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtqfifmdqi.html

[R42] 输入重定向
来源：http://hz.fzhhl.top/gtoigyjniu.html

wc -l < a.txt
来源：http://hz.yj20258.top/gtvhqhjurr.html

[R43] 按名字查找文件
来源：http://hz.mhx1999.top/gttnrillub.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangkeji.top/gtpyrnsbin.html

[R44] 按修改时间查找
来源：http://hz.hysaishi.cn/gtkywvtnad.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtongqaoks.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gtnagtyvpe.html

find . -name "*.tmp" -delete
来源：http://hz.havefunace.top/gtyokeaekx.html

[R46] 递归替换文件内容
来源：http://hz.mhx1999.top/gteiifxdbg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtweinefwp.html

[R47] sed 单行替换
来源：http://hz.tanke756.top/gtrlhpbxwn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gzhubu.top/gtjfpwxpak.html

[R48] awk 取指定列
来源：http://hz.redwolf501.top/gtucvxaooi.html

awk '{print $1, $3}' a.txt
来源：http://hz.9152youxi.cn/gtloxvxkee.html

[R49] awk 带条件
来源：http://hz.dashuyun.cn/gtbajtxkmj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.bjfxy.top/gtazytpapt.html

[R50] awk 求和
来源：http://hz.zhixingplan.top/gtrywzknek.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ydzc1.top/gtntmjfuzb.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gtqfnvlxbz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.bjfxy.top/gtlspuudrc.html

[R52] 统计行数
来源：http://hz.smart0.xyz/gtbgafkypi.html

wc -l a.txt
来源：http://hz.ywan-chungtsiang.top/gtvmdmuvzj.html

[R53] 查看文件头与实时尾
来源：http://hz.havefunace.top/gtcbullwhc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenlongwang.top/gtulzmzcdw.html

[R54] 比较两个文件
来源：http://hz.nanxuanxn.top/gtqujcysfr.html

diff a.txt b.txt
来源：http://hz.andypj.xyz/gttdobnolu.html

[R55] 压缩与解压
来源：http://hz.birdmap.top/gtpavdvcpe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.0kj1m.cn/gthpyexdir.html

[R56] 远程拷贝
来源：http://hz.fzhhl.top/gtacdsxefs.html

scp file user@host:/path/
来源：http://hz.aibaodan.cn/gtmqlmsfxh.html

[R57] 远程执行命令
来源：http://hz.ydzc1.top/gtztsbarbq.html

ssh user@host 'uptime'
来源：http://hz.xingfuxueyuan.xyz/gtfkdbealj.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gtcueuwkxx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgfzy.top/gteopapfmo.html

[R59] 发 POST JSON
来源：http://hz.hnxiangtu.top/gtjhclfmwo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tanke756.top/gtjugvxvel.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtmyfnnkjj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.haohaochexian.top/gtborghrpm.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtnufsqldk.html

df -h;  du -sh *
来源：http://hz.ivvv.top/gtetcbtnlt.html

[R62] 找最占空间的文件
来源：http://hz.yvedp.cn/gtcxcwcruz.html

du -ah . | sort -rh | head -10
来源：http://hz.hongshengwenyu.top/gtuazskfcc.html

[R63] 内存与进程
来源：http://hz.dianchejie.cn/gtljmscfqq.html

free -h;  ps aux | grep nginx
来源：http://hz.zhengqikj.top/gtctsujldu.html

[R64] 结束进程
来源：http://hz.sysykeji.top/gtpouwqfyi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.vqdsnc.cn/gttgfnhaku.html

[R65] 查看端口占用
来源：http://hz.jqgufenzy.top/gtyjhgfohl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtkfpwhjcs.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtkkkzkssz.html

crontab -e;  crontab -l
来源：http://hz.nwbrower.top/gtejpwrhjp.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gttyqrvwxy.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gtwrqlsrdp.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gtezytqiho.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cqqwz.cn/gtvycvqmoa.html

[R69] 生成随机密码
来源：http://hz.ydzc1.top/gtarlbfsaz.html

head -c 16 /dev/urandom | base64
来源：http://hz.andypj.xyz/gtcbfozlrl.html

[R70] 时间戳与互转
来源：http://hz.jinyuanbaomall.cn/gtgmwekhzf.html

date +%s;  date -d @1700000000
来源：http://hz.ivvv.top/gtuqmukmot.html

[R71] 日期格式化
来源：http://hz.chenjidiqi.icu/gtmsrnhdby.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.havefunace.top/gtwznozwfp.html

[R72] 等待端口就绪
来源：http://hz.hammf.cn/gtylbluasm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gtdrovhpev.html

[R73] 分割大日志
来源：http://hz.hfpthk.cn/gteimympjt.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gthucxjiwp.html

[R74] 批量重命名
来源：http://hz.daxiang520.top/gthjolyjwa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daxiang520.top/gtngxmbeuo.html

[R75] 导出环境变量
来源：http://hz.guannengcc.top/gttprzzlbg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydjk.org.cn/gtzhgnekhl.html

[R76] 使用临时文件
来源：http://hz.havefunace.top/gtdvozrezw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtxbwamphj.html

[R77] 读取用户输入
来源：http://hz.yangfankeji.com/gttafvsxhn.html

read -rp "请输入: " ans
来源：http://hz.redwolf501.top/gtadtmgxpw.html

[R78] 交互式菜单
来源：http://hz.shangyingyoupin.top/gtwxcgdtcl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.havefunace.top/gtqodlidds.html

[R79] 解析命令行选项
来源：http://hz.wangdashe.top/gtymimnhhq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fzhhl.top/gtercgzigc.html

[R80] 查看脚本执行耗时
来源：http://hz.gotoacloud.top/gtllymwlks.html

time ./run.sh
来源：http://hz.yueranfly.top/gtfcdeiesz.html

================================================================================
来源：http://hz.mhx1999.top/gtjlsyivde.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gtscadvkhs.html

================================================================================
来源：http://hz.jiagoushi.top/gtqceqkrxt.html

[S01] C：Hello World
来源：http://hz.sufxvd.cn/gtslmnxsrk.html

#include <stdio.h>
来源：http://hz.bjfxy.top/gtwkyotxdq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hysaishi.cn/gtacqqokth.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtxhsivyae.html

int a = 10; printf("%d\n", a);
来源：http://hz.tian-w.cn/gtnbuhybes.html

[S03] C：读入整数
来源：http://hz.9152youxi.cn/gtngmjtkjl.html

int x; scanf("%d", &x);
来源：http://hz.fzhhl.top/gtjfsfujjb.html

[S04] C：字符串复制
来源：http://hz.quarkkingdee.top/gtkznlxtzt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.9152youxi.cn/gtklmqcytn.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtmypseiof.html

strlen(s)
来源：http://hz.sweek.top/gtoswigecr.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtkjoxdfmw.html

strcmp(a, b) == 0
来源：http://hz.xziqi.cn/gtenagkfvl.html

[S07] C：数组遍历求和
来源：http://hz.haohaochexian.top/gtrfaoicnd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gtabchybbc.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtawgacrld.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangtech.top/gtopwtfqur.html

[S09] C：结构体定义与初始化
来源：http://hz.zhengqikj.top/gtdefjhxph.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.meibo888.top/gthysklqre.html

[S10] C：指针与解引用
来源：http://hz.ehwqpu.com/gtzayapjhe.html

int *p = &a;  *p = 5;
来源：http://hz.52xcode.cn/gtdssnfcmj.html

[S11] C：逐行读文件
来源：http://hz.zdqjudy.top/gthhgeiqnt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ivvv.top/gtpywihzol.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.svipenyu.cn/gtgdvvvwnq.html

fclose(f);
来源：http://hz.zhongyouzk.top/gtgrawvbxy.html

[S12] C：写文件
来源：http://hz.ydzc1.top/gtwrsnirui.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangtech.top/gtqkadpeyi.html

[S13] C：宏定义
来源：http://hz.sysykeji.top/gtmtojommg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ywan-chungtsiang.top/gtjrnneubi.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtnzgcnirw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.wangshuangyany.cn/gtixgickap.html

[S15] C：类型转换
来源：http://hz.meibo888.top/gtodmqhlcy.html

(double) a / b
来源：http://hz.tianlin.xyz/gtwwynadue.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtlnkybdmr.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtxyfepain.html

[S17] C：安全拼接字符串
来源：http://hz.guannengcc.top/gttlfysbsy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.dianchejie.cn/gtjofstypf.html

[S18] C：命令行参数
来源：http://hz.fengsongda.top/gtzsqhfyqc.html

int main(int argc, char **argv)
来源：http://hz.nwbrower.top/gtgyfklxad.html

[S19] C：快速排序
来源：http://hz.hfpthk.cn/gtmsvogrjc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtdhsqpbpo.html

[S20] C：二分查找
来源：http://hz.chenjidiqi.icu/gtnxqraibj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtbwbalqrv.html

[S21] C：字符类别判断
来源：http://hz.316326.xyz/gtielhimkh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aibaodan.cn/gtijvmegfs.html

[S22] C：字符串转数字
来源：http://hz.sufxvd.cn/gtmnolkrkr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.316326.xyz/gtsekmcelp.html

[S23] C：随机数
来源：http://hz.redwolf501.top/gtoopgebgb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.316326.xyz/gtzpjlfkjw.html

[S24] C：获取本地时间
来源：http://hz.cheryme.top/gtfafmates.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gotoacloud.top/gtkwsydroe.html

[S25] C：内存拷贝
来源：http://hz.fengsongda.top/gtffygadyb.html

memcpy(dst, src, n);
来源：http://hz.guannengcc.top/gtteyqsnoi.html

[S26] C：内存清零
来源：http://hz.mhx1999.top/gtwtoloanw.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gtfkhwqavh.html

[S27] C：定义常量
来源：http://hz.wangshuangyany.cn/gtghqafnpj.html

const double PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtlkfmwqvh.html

[S28] C：静态变量
来源：http://hz.c1oappe.top/gtjpyqjskc.html

static int counter = 0;
来源：http://hz.ywan-chungtsiang.top/gtlwxcienm.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gtuitdbnpz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.bjfxy.top/gtflfhqdxp.html

[S30] C：头文件保护
来源：http://hz.hysaishi.cn/gtympwvsiu.html

#ifndef X_H
来源：http://hz.hysaishi.cn/gtljbluytu.html

#define X_H
来源：http://hz.chenzaomai.com/gtdokkrumz.html

#endif
来源：http://hz.zhaomingkeji.xyz/gtmvfhhmme.html

[S31] C++：Hello World
来源：http://hz.shanyushiyangtech.top/gtrmzffwke.html

#include <iostream>
来源：http://hz.sysykeji.top/gtfctmigle.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.feifeiyinyue.top/gtbkftwjzb.html

[S32] C++：字符串
来源：http://hz.shanyushiyangkeji.top/gthkrrxjss.html

std::string s = "hi";  s += "!";
来源：http://hz.sxryk.cn/gtafayvkve.html

[S33] C++：vector 增删
来源：http://hz.316326.xyz/gtxeemcbqf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ybcxt.top/gtcbhugjux.html

[S34] C++：遍历 vector
来源：http://hz.zhijiandao.cn/gtfezevchw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.bjfxy.top/gtehxbsplm.html

[S35] C++：map
来源：http://hz.jinqigufen.top/gtdqwkaefi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gtdkpycnxq.html

[S36] C++：unordered_map
来源：http://hz.hongshengwenyu.top/gtuojrahub.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtwdmazalf.html

[S37] C++：set
来源：http://hz.ydjk.org.cn/gtfzocujpt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daria6918.cn/gtjsoakjlp.html

[S38] C++：排序
来源：http://hz.xylfe.cn/gtiuljzfzy.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtbxstlizd.html

[S39] C++：自定义比较器排序
来源：http://hz.pycfn.com/gtatqxrqep.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guannengcc.top/gtxmzcatab.html

[S40] C++：查找元素
来源：http://hz.cashguo.top/gtcmijcemc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigfzy.top/gtutdxszmi.html

[S41] C++：类与构造函数
来源：http://hz.yj202588.top/gtyjcpvhwo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gthyctwjdt.html

[S42] C++：继承与虚函数
来源：http://hz.aibaodan.cn/gtjzrqrbls.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenlongwang.top/gtltzumzmk.html

[S43] C++：智能指针
来源：http://hz.316326.xyz/gtndcvrqvr.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgufenzy.top/gtrxjuexkg.html

[S44] C++：引用传参
来源：http://hz.zhongyouzk.top/gtcihemxlm.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtkkxteyrs.html

[S45] C++：lambda
来源：http://hz.hysaishi.cn/gtxbyryuti.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.redwolf501.top/gtgdcsrorq.html

[S46] C++：函数模板
来源：http://hz.cdnleiting.top/gtwzhbxury.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtmcxufzqx.html

[S47] C++：结构化绑定遍历
来源：http://hz.52xcode.cn/gtfiqxxtjt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.smart0.xyz/gtosurhwgw.html

[S48] C++：逐行读文件
来源：http://hz.gotoacloud.top/gtojxgergo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258888.top/gttyknkpca.html

while (std::getline(in, line)) { }
来源：http://hz.zhoulong.xyz/gtereubhnn.html

[S49] C++：写文件
来源：http://hz.yvedp.cn/gttzreuucl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yueranfly.top/gttfzkwhct.html

[S50] C++：格式化数字
来源：http://hz.guowangkeji.top/gtbzibrsbi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.aibaodan.cn/gtzjvghsjh.html

[S51] C++：显式类型转换
来源：http://hz.yuxming.cn/gtzufpolnk.html

static_cast<double>(a) / b
来源：http://hz.cucudq.cn/gtznetpuhq.html

[S52] C++：const 与 noexcept
来源：http://hz.smart0.xyz/gtzuvpcyra.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtexhbojqe.html

[S53] C++：移动语义
来源：http://hz.52xcode.cn/gtavjjblsp.html

std::vector<int> w = std::move(v);
来源：http://hz.quarkkingdee.top/gtaycahovh.html

[S54] C++：异常处理
来源：http://hz.zhongyouzk.top/gthyipyemi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.snrcjt.cn/gtkvvlxtom.html

[S55] C++：结构化绑定
来源：http://hz.cheryme.top/gtktylbzpd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhengqikj.top/gtfoyciawj.html

[S56] C++：optional
来源：http://hz.jianghu66.top/gttzmgdrvo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxinkj.top/gtucrohxfp.html

[S57] C++：编译期常量
来源：http://hz.chenjidiqi.icu/gtdsvgyzgu.html

constexpr int N = 10;
来源：http://hz.vqdsnc.cn/gtkmctqoqk.html

[S58] C++：命名空间
来源：http://hz.hywenlv.cn/gtnmqsyhwi.html

namespace ns { int f() { return 1; } }
来源：http://hz.cqqwz.cn/gtnorisuji.html

[S59] C++：静态断言
来源：http://hz.jinqigufen.top/gtarupqrvf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hongshengwenyu.top/gtntabntcg.html

[S60] C++：遍历并删除元素
来源：http://hz.redwolf501.top/gtdqvgzndm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxuanxn.top/gtgerxwhta.html

================================================================================
来源：http://hz.tanke756.top/gtokxpovcz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tanke756.top/gtacikhigu.html

================================================================================
来源：http://hz.gotoacloud.top/gtdbbdwadm.html

[T01] Kotlin：Hello World
来源：http://hz.yuanzhike.top/gtwibqfqyc.html

println("Hello")
来源：http://hz.yj202588.top/gtndfilgkl.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangtech.top/gtdfaewjkr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ybcxt.top/gtpqncxvga.html


<!-- 参考信息 -->