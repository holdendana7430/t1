代发 wailian999

readonly PI=3.14
来源：http://hz.feifeiyinyue.top/gtadqtjmzz.html

[R04] 位置参数
来源：http://hz.shanyushiyangtech.top/gteeuutcny.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuanzx.com/gtuturylnw.html

[R05] 参数默认值
来源：http://hz.hysaishi.cn/gtfliguulx.html

name="${1:-default}"
来源：http://hz.tianlin.xyz/gtmfmqcnha.html

[R06] 判断命令是否存在
来源：http://hz.xingfuxueyuan.xyz/gtwmpxakxt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtchnrhtgp.html

[R07] if 判断文件
来源：http://hz.yvedp.cn/gtycbrswbm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sxryk.cn/gtknqxrfhm.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtvohtjhqd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.feifeiyinyue.top/gtctwqgygk.html

[R09] 字符串比较
来源：http://hz.daxiang520.top/gtbdikkoyv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aizwys.cn/gtfdsdjmpa.html

[R10] 正则匹配
来源：http://hz.fzhhl.top/gtfagyqaha.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgufenzy.top/gtqdbnpmkd.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtwtnxamzu.html

case "$1" in
来源：http://hz.chenzaomai.com/gttcflsrlc.html

start) echo "启动" ;;
来源：http://hz.chenzaomai.com/gtdrvbunhs.html

stop)  echo "停止" ;;
来源：http://hz.xylfe.cn/gtysmfgeow.html

*)     echo "未知命令" ;;
来源：http://hz.xuanzx.com/gtmevitwot.html

esac
来源：http://hz.yangfankeji.com/gtsradzdqd.html

[R12] for 遍历文件
来源：http://hz.dashuyun.cn/gtjwnduzwb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gtqtldctbx.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtgvewamzr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.mhx1999.top/gtscxqdezj.html

[R14] C 风格 for
来源：http://hz.sysykeji.top/gtyowvmaxf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtqombpjcr.html

[R15] while 逐行读文件
来源：http://hz.c1oappe.top/gthizrpsev.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258.top/gtkivbzqqd.html

[R16] until 等待条件
来源：http://hz.zhiwuduotai.top/gtgsdloicq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtgiktmctk.html

[R17] 数组定义与取值
来源：http://hz.quarkkingdee.top/gtpolstsgq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.dashuyun.cn/gtbzgidlxc.html

[R18] 遍历数组
来源：http://hz.gotoacloud.top/gtggtrsrfm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gthypksbun.html

[R19] 数组长度
来源：http://hz.yuxming.cn/gtigljjvyk.html

echo "${#arr[@]}"
来源：http://hz.yvedp.cn/gtksxqmgkt.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gtlifmvcst.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.haohaochexian.top/gtcoykwtql.html

[R21] 字符串长度
来源：http://hz.chenzaomai.com/gtzxuwfotg.html

echo "${#s}"
来源：http://hz.yuxming.cn/gtcwqktyrp.html

[R22] 截取子串
来源：http://hz.cdnleiting.top/gttagtwypz.html

echo "${s:0:5}"
来源：http://hz.c1oappe.top/gtswyzqizr.html

[R23] 字符串替换
来源：http://hz.fzhhl.top/gtimoksioq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yongpay.top/gtufeokoxx.html

[R24] 大小写转换
来源：http://hz.fzhhl.top/gtxnjhwpga.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxinkj.top/gtbjexsdqk.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuanzhike.top/gtnumokjvd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtosdswlvf.html

[R26] 命令替换
来源：http://hz.chenlongwang.top/gtdzakbaog.html

now=$(date +%F); echo "$now"
来源：http://hz.haohaochexian.top/gtaujyquht.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtieouwwan.html

echo $((1 + 2 * 3))
来源：http://hz.xuetiantiany.cn/gtzygezbrd.html

[R28] 浮点运算
来源：http://hz.xinyue.icu/gtinqqhwge.html

echo "scale=2; 10/3" | bc
来源：http://hz.kuanghao11.cn/gtfgjcdphg.html

[R29] 定义函数
来源：http://hz.hnqzz.top/gtktnecvtm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenjidiqi.icu/gtejsamjgq.html

[R30] 函数返回状态码
来源：http://hz.cashguo.top/gtbfgnripk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtgjknqrlz.html

[R31] 局部变量
来源：http://hz.ehwqpu.com/gtkijlnrpc.html

f() { local x=1; echo "$x"; }
来源：http://hz.hfpthk.cn/gtsqtlyxaq.html

[R32] 参数个数校验
来源：http://hz.sysykeji.top/gtfyfivvzc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zycfv.cn/gtzkeupohj.html

[R33] 捕获错误并提示行号
来源：http://hz.shzxlz.cn/gtkhaliqhe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangtech.top/gtqnltzmph.html

[R34] 退出时清理
来源：http://hz.dianchejie.cn/gtjtpzvjry.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtetttkdzq.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtghmlnzss.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenlongwang.top/gtimmopede.html

[R36] 并发执行多个任务
来源：http://hz.0kj1m.cn/gtekuklees.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gzhubu.top/gtrmxlicvj.html

[R37] 把输出赋给变量
来源：http://hz.daria6918.cn/gtlzqlamjr.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtjrptfdxu.html

[R38] 管道串联
来源：http://hz.cheryme.top/gtixuebnuh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hongshengwenyu.top/gtpctzojbs.html

[R39] 重定向标准输出与错误
来源：http://hz.zhaomingkeji.xyz/gtlosleaeo.html

cmd > out.log 2>&1
来源：http://hz.9152youxi.cn/gteeufktow.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtjjkyudrn.html

echo "log" >> out.log
来源：http://hz.yj202588.top/gtlvnpbfpk.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtjyhomldr.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtgqorfucr.html

[R42] 输入重定向
来源：http://hz.aibaodan.cn/gthkqjhict.html

wc -l < a.txt
来源：http://hz.cashguo.top/gtrttokcmf.html

[R43] 按名字查找文件
来源：http://hz.jiagoushi.top/gtbstdkkuu.html

find . -name "*.log" -type f
来源：http://hz.zhixingplan.top/gthogxqtyo.html

[R44] 按修改时间查找
来源：http://hz.yuxming.cn/gtufzyfayd.html

find . -mtime -7 -type f
来源：http://hz.vqdsnc.cn/gtylrxkvhc.html

[R45] 批量删除
来源：http://hz.ybcxt.top/gtczwgrrxd.html

find . -name "*.tmp" -delete
来源：http://hz.hnqzz.top/gtmjyogbra.html

[R46] 递归替换文件内容
来源：http://hz.tianlin.xyz/gtwutefret.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxinkj.top/gtdntifrmq.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtjpnzqdol.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gthnjsrnbz.html

[R48] awk 取指定列
来源：http://hz.sxryk.cn/gtkcegzfvf.html

awk '{print $1, $3}' a.txt
来源：http://hz.andypj.xyz/gtwyypkpxz.html

[R49] awk 带条件
来源：http://hz.xingfuxueyuan.xyz/gtqhjuugbm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.iojbl.cn/gtonxtoodb.html

[R50] awk 求和
来源：http://hz.redwolf501.top/gtxwurvfyj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zdqjudy.top/gtjwyehmsc.html

[R51] 排序去重取前几
来源：http://hz.zhoulong.xyz/gtcxjglfrb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtlzadmitw.html

[R52] 统计行数
来源：http://hz.jqgufenzy.top/gtojosarfu.html

wc -l a.txt
来源：http://hz.gzhubu.top/gtxknzsevp.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtuyvzaugc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtzbehbaju.html

[R54] 比较两个文件
来源：http://hz.ehwqpu.com/gtktvtegnw.html

diff a.txt b.txt
来源：http://hz.havefunace.top/gtdqmtseas.html

[R55] 压缩与解压
来源：http://hz.jinghuilouyu.cn/gtttyhzath.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zdqjudy.top/gtcwmtwtwf.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gtucunqhah.html

scp file user@host:/path/
来源：http://hz.cashguo.top/gtvubxkedl.html

[R57] 远程执行命令
来源：http://hz.zhongyouzk.top/gtpiucsueb.html

ssh user@host 'uptime'
来源：http://hz.andypj.xyz/gtxokeczmb.html

[R58] 下载文件
来源：http://hz.vqdsnc.cn/gtxyjqdmdl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinyuanbaomall.cn/gtfryolfne.html

[R59] 发 POST JSON
来源：http://hz.chenjidiqi.icu/gtoulqnntp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hfpthk.cn/gtuhjeukue.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtkgpxubnz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gtafthfaxl.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtutfmewcn.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gtssssungd.html

[R62] 找最占空间的文件
来源：http://hz.yongpay.top/gtkbiccipq.html

du -ah . | sort -rh | head -10
来源：http://hz.feifeiyinyue.top/gtogfrzscd.html

[R63] 内存与进程
来源：http://hz.hysaishi.cn/gtpugmbjfw.html

free -h;  ps aux | grep nginx
来源：http://hz.shuidangran.top/gtzhycncwr.html

[R64] 结束进程
来源：http://hz.hysaishi.cn/gtfpmjgvwe.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhoulong.xyz/gtxrugdzqm.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gtannzpjid.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtufnichhk.html

[R66] 定时任务
来源：http://hz.jinghuilouyu.cn/gteldvbwvc.html

crontab -e;  crontab -l
来源：http://hz.yueranfly.top/gtnczcphxn.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtbarvcicl.html

openssl rand -hex 16
来源：http://hz.nwbrower.top/gtpfwprkth.html

[R68] 计算文件校验值
来源：http://hz.xingfuxueyuan.xyz/gtodxsjfwn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cucudq.cn/gthmspbgxr.html

[R69] 生成随机密码
来源：http://hz.cucudq.cn/gtrffvldjz.html

head -c 16 /dev/urandom | base64
来源：http://hz.yongpay.top/gtzfgiqhwt.html

[R70] 时间戳与互转
来源：http://hz.shzxlz.cn/gtmpijguom.html

date +%s;  date -d @1700000000
来源：http://hz.tian-w.cn/gtbvnvzxmt.html

[R71] 日期格式化
来源：http://hz.daxiang520.top/gtrfynfziq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fengsongda.top/gtjrmptgxh.html

[R72] 等待端口就绪
来源：http://hz.xuetiantiany.cn/gtxbxjatpj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yangfankeji.com/gtyizwkljj.html

[R73] 分割大日志
来源：http://hz.shzxlz.cn/gtqkzailox.html

split -l 1000 big.log part_
来源：http://hz.xuetiantiany.cn/gtjcbeusoz.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtzxislxlm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dashuyun.cn/gtvtgaxrpn.html

[R75] 导出环境变量
来源：http://hz.zhoulong.xyz/gtpbavtfgs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gaohongyu789.top/gtbhnafgmz.html

[R76] 使用临时文件
来源：http://hz.fengsongda.top/gtbgqrxeju.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.fengsongda.top/gtjsyodoxt.html

[R77] 读取用户输入
来源：http://hz.ydzc1.top/gtqpnjptrv.html

read -rp "请输入: " ans
来源：http://hz.dianchejie.cn/gttlddqvcb.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtncbkalne.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shuidangran.top/gtfgndezwk.html

[R79] 解析命令行选项
来源：http://hz.yvedp.cn/gtwmitsohu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gtyrmnrcks.html

[R80] 查看脚本执行耗时
来源：http://hz.mhx1999.top/gtjobsmrcy.html

time ./run.sh
来源：http://hz.tian-w.cn/gtaayjprdc.html

================================================================================
来源：http://hz.hfpthk.cn/gtatgefnic.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gthkiplbku.html

================================================================================
来源：http://hz.dianchejie.cn/gtruwzuaxs.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtdewubtko.html

#include <stdio.h>
来源：http://hz.hnqzz.top/gtxnwexmex.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xinyue.icu/gtcmdfhlpm.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gtfrxtyguq.html

int a = 10; printf("%d\n", a);
来源：http://hz.yueranfly.top/gtosygobva.html

[S03] C：读入整数
来源：http://hz.fengsongda.top/gtusdelwin.html

int x; scanf("%d", &x);
来源：http://hz.gaohongyu789.top/gtrjekwcvz.html

[S04] C：字符串复制
来源：http://hz.yuxming.cn/gtkxvxmxgv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gotoacloud.top/gtutczpglu.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtugcqjigc.html

strlen(s)
来源：http://hz.vqdsnc.cn/gtzojoxekz.html

[S06] C：字符串比较
来源：http://hz.kuanghao11.cn/gtmiinubvn.html

strcmp(a, b) == 0
来源：http://hz.nwbrower.top/gtutbfnyjp.html

[S07] C：数组遍历求和
来源：http://hz.zhoulong.xyz/gtvukpgaco.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.mhx1999.top/gtdsasyoxt.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258888.top/gtlwjmjnzn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuetiantiany.cn/gtowmmrlmn.html

[S09] C：结构体定义与初始化
来源：http://hz.jinghuilouyu.cn/gtfhmztlxb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nanxuanxn.top/gtdltxpevi.html

[S10] C：指针与解引用
来源：http://hz.jinghuilouyu.cn/gtroxtatus.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gthiemognu.html

[S11] C：逐行读文件
来源：http://hz.kuanghao11.cn/gtqkozbuip.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yvedp.cn/gtrtrcqguc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ehwqpu.com/gtmjcstzbi.html

fclose(f);
来源：http://hz.wangshuangyany.cn/gtdheyladn.html

[S12] C：写文件
来源：http://hz.pengpengdd.cyou/gtwsfpqope.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.feifeiyinyue.top/gtztgnjhsq.html

[S13] C：宏定义
来源：http://hz.svipenyu.cn/gtozvjsved.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zycfv.cn/gtcxhjeswl.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtbgocmxjz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cqqwz.cn/gtaebdspit.html

[S15] C：类型转换
来源：http://hz.dianchejie.cn/gtkvdqjeep.html

(double) a / b
来源：http://hz.hnxiangtu.top/gtxfpcyhyk.html

[S16] C：位操作置位
来源：http://hz.yuanzhike.top/gtxxmzlvgq.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtqnjfzfcq.html

[S17] C：安全拼接字符串
来源：http://hz.sxryk.cn/gtpfffqxwi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gzhubu.top/gtwvhgztcx.html

[S18] C：命令行参数
来源：http://hz.xuetiantiany.cn/gtmkmwicvb.html

int main(int argc, char **argv)
来源：http://hz.sysykeji.top/gtkztcirda.html

[S19] C：快速排序
来源：http://hz.guannengcc.top/gtmushlmin.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yongpay.top/gtoceghxem.html

[S20] C：二分查找
来源：http://hz.jqgufenzy.top/gtmcqwvhip.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gtqqnsorgx.html

[S21] C：字符类别判断
来源：http://hz.hnqzz.top/gtmvpnlvec.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shanyushiyangkeji.top/gtwluenvtp.html

[S22] C：字符串转数字
来源：http://hz.jiagoushi.top/gtwqgnzovm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtdetqvycn.html

[S23] C：随机数
来源：http://hz.yueranfly.top/gtxpyqrqjj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yvedp.cn/gtrftktmmc.html

[S24] C：获取本地时间
来源：http://hz.tian-w.cn/gtpqoozzrm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gtaqtyantc.html

[S25] C：内存拷贝
来源：http://hz.svipenyu.cn/gttxywltpr.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtgdwcyzoq.html

[S26] C：内存清零
来源：http://hz.hywenlv.cn/gtjoyafdqq.html

memset(a, 0, sizeof a);
来源：http://hz.birdmap.top/gtglnfppkk.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtjdiaoplj.html

const double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gteskzyijn.html

[S28] C：静态变量
来源：http://hz.xuetiantiany.cn/gtxggymuxm.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtctagixyh.html

[S29] C：变参函数
来源：http://hz.andypj.xyz/gtsxiemlrm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gaohongyu789.top/gtjvhkiimy.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gtjyzfxxlb.html

#ifndef X_H
来源：http://hz.aibaodan.cn/gtypsqjydz.html

#define X_H
来源：http://hz.sweek.top/gtfacgcxms.html

#endif
来源：http://hz.shanyushiyangtech.top/gttxdrbmrd.html

[S31] C++：Hello World
来源：http://hz.mhx1999.top/gtffpmxspz.html

#include <iostream>
来源：http://hz.nwbrower.top/gtrondnbej.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xingfuxueyuan.xyz/gtdfzjzgkj.html

[S32] C++：字符串
来源：http://hz.ehwqpu.com/gthqdleiyg.html

std::string s = "hi";  s += "!";
来源：http://hz.feifeiyinyue.top/gtbwlevoyw.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gtwvjamwqx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtliysudyg.html

[S34] C++：遍历 vector
来源：http://hz.hnqzz.top/gtpagfrxnz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gtjcthcrqt.html

[S35] C++：map
来源：http://hz.jqgufenzy.top/gtxtberajp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gtnncmtpnd.html

[S36] C++：unordered_map
来源：http://hz.tianlin.xyz/gtavhhzmrq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtbnywhiwm.html

[S37] C++：set
来源：http://hz.ydzc1.top/gtrfcwsdby.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guowangkeji.top/gthnhwlmcy.html

[S38] C++：排序
来源：http://hz.zdqjudy.top/gtfpaxpbov.html

std::sort(v.begin(), v.end());
来源：http://hz.daxiang520.top/gtynsmnpmb.html

[S39] C++：自定义比较器排序
来源：http://hz.ppjwa.cn/gtvqiuwant.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hysaishi.cn/gtaynkjxkq.html

[S40] C++：查找元素
来源：http://hz.andypj.xyz/gtbfjszpme.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yangfankeji.com/gtkuyzlxak.html

[S41] C++：类与构造函数
来源：http://hz.yuanzhike.top/gtjizhwhud.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj202588.top/gtohewchmj.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtunkhymro.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtgiefphyw.html

[S43] C++：智能指针
来源：http://hz.iojbl.cn/gtmtbthxzw.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxuanxn.top/gtmnatpgpf.html

[S44] C++：引用传参
来源：http://hz.0kj1m.cn/gtmwmrtxbc.html

void inc(int &x) { ++x; }
来源：http://hz.pycfn.com/gtzjlorejp.html

[S45] C++：lambda
来源：http://hz.haohaochexian.top/gtnomyecde.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtuvgjqzyx.html

[S46] C++：函数模板
来源：http://hz.cqqwz.cn/gtltiafsie.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtbmtauroi.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenjidiqi.icu/gtmzggrldo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hywenlv.cn/gtvcflbaai.html

[S48] C++：逐行读文件
来源：http://hz.shzxlz.cn/gtjvqimbde.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtmsqqslvb.html

while (std::getline(in, line)) { }
来源：http://hz.snrcjt.cn/gtliramdvq.html

[S49] C++：写文件
来源：http://hz.jqgfzy.top/gtuyekdfmv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aizwys.cn/gtpwjobvgp.html

[S50] C++：格式化数字
来源：http://hz.ywan-chungtsiang.top/gtswatooea.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.svipenyu.cn/gtscokvecr.html

[S51] C++：显式类型转换
来源：http://hz.snrcjt.cn/gtkbpzkvcj.html

static_cast<double>(a) / b
来源：http://hz.xinyue.icu/gttcykawmz.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258.top/gtmtzjnfcj.html

int size() const noexcept { return n_; }
来源：http://hz.guowangkeji.top/gtuiudlofx.html

[S53] C++：移动语义
来源：http://hz.feifeiyinyue.top/gtpricquiu.html

std::vector<int> w = std::move(v);
来源：http://hz.pycfn.com/gtzwnomlft.html

[S54] C++：异常处理
来源：http://hz.nanxuanxn.top/gtmlhnsmmp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydjk.org.cn/gtuxxyjdeh.html

[S55] C++：结构化绑定
来源：http://hz.tianlin.xyz/gtuqanbfde.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.kuanghao11.cn/gtxbkxtbla.html

[S56] C++：optional
来源：http://hz.smart0.xyz/gttwidsevb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinyuanbaomall.cn/gtlolmzbps.html

[S57] C++：编译期常量
来源：http://hz.fengsongda.top/gtafwzvtti.html

constexpr int N = 10;
来源：http://hz.shuidangran.top/gtiotnmdzo.html

[S58] C++：命名空间
来源：http://hz.jqgfzy.top/gtqcvyartv.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtsvqinvvn.html

[S59] C++：静态断言
来源：http://hz.andypj.xyz/gttkpplqol.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.snrcjt.cn/gtpxtqhkjk.html

[S60] C++：遍历并删除元素
来源：http://hz.ppjwa.cn/gtyhmokbhw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258888.top/gtatuiyjzl.html

================================================================================
来源：http://hz.vqdsnc.cn/gtezkutbjx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtfcxuaaxt.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmptgjwdu.html

[T01] Kotlin：Hello World
来源：http://hz.xylfe.cn/gthjvtoqud.html

println("Hello")
来源：http://hz.meibo888.top/gttrosvlub.html

[T02] Kotlin：变量
来源：http://hz.shuidangran.top/gtnalontsk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gzhubu.top/gtbexrfxxs.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangkeji.top/gtlawuaicn.html

"值: $b"
来源：http://hz.nwbrower.top/gtnftpalkt.html

[T04] Kotlin：空安全
来源：http://hz.tanke756.top/gtqvdpophn.html

val n: String? = null;  n?.length
来源：http://hz.xinyue.icu/gtgayxvpam.html


<!-- 参考信息 -->