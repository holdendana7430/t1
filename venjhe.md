代发 wailian999

name="${1:-default}"
来源：http://hz.cdnleiting.top/gtkhbrbsil.html

[R06] 判断命令是否存在
来源：http://hz.aizwys.cn/gtrfmjbqan.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtumveoxla.html

[R07] if 判断文件
来源：http://hz.yongpay.top/gtruchpmoe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sxryk.cn/gtcayefmbf.html

[R08] 数值比较
来源：http://hz.hongshengwenyu.top/gtcdlecjou.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xylfe.cn/gthycwqbwc.html

[R09] 字符串比较
来源：http://hz.tianlin.xyz/gtyenbsfjf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.0kj1m.cn/gtirvmzmdh.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gthygucgsw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zycfv.cn/gtixludpch.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtfjhkuwoi.html

case "$1" in
来源：http://hz.tianlin.xyz/gtakdtexda.html

start) echo "启动" ;;
来源：http://hz.shzxlz.cn/gtxxsvcxbm.html

stop)  echo "停止" ;;
来源：http://hz.daxiang520.top/gtjyonvcoc.html

*)     echo "未知命令" ;;
来源：http://hz.wangdashe.top/gthkufytmp.html

esac
来源：http://hz.xuetiantiany.cn/gtcbwgyfdm.html

[R12] for 遍历文件
来源：http://hz.ivvv.top/gtucfqglya.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aizwys.cn/gtzqntqhjb.html

[R13] for 计数循环
来源：http://hz.quarkkingdee.top/gtxzlpyjgm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yongpay.top/gtnvjnloex.html

[R14] C 风格 for
来源：http://hz.bjfxy.top/gtiviibwkf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtnayxstkp.html

[R15] while 逐行读文件
来源：http://hz.zhaomingkeji.xyz/gttwdwftyz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenjidiqi.icu/gtnccyyvqy.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtnmvxlwas.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtfpzskddw.html

[R17] 数组定义与取值
来源：http://hz.yangfankeji.com/gthlmgrxcz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sysykeji.top/gtghoxygzg.html

[R18] 遍历数组
来源：http://hz.zycfv.cn/gtysattrsa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tanke756.top/gtaxcyhpez.html

[R19] 数组长度
来源：http://hz.fzhhl.top/gteeyafccw.html

echo "${#arr[@]}"
来源：http://hz.ivvv.top/gtuhhffttv.html

[R20] 关联数组（字典）
来源：http://hz.jinqigufen.top/gtqdgcykvd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ivvv.top/gtdqbztwuf.html

[R21] 字符串长度
来源：http://hz.snrcjt.cn/gttdkjfqdp.html

echo "${#s}"
来源：http://hz.zhoulong.xyz/gtygopxsln.html

[R22] 截取子串
来源：http://hz.jinghuilouyu.cn/gtrfctucoz.html

echo "${s:0:5}"
来源：http://hz.ydjk.org.cn/gtmqvpbzdv.html

[R23] 字符串替换
来源：http://hz.smart0.xyz/gtgoeedlhr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangkeji.top/gtdycwwhnq.html

[R24] 大小写转换
来源：http://hz.ehwqpu.com/gteribshnh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sxryk.cn/gtibiohmnq.html

[R25] 去后缀 / 去前缀
来源：http://hz.shzxlz.cn/gtaadmxptk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhaomingkeji.xyz/gtyhperndw.html

[R26] 命令替换
来源：http://hz.hammf.cn/gtjhjrbzjf.html

now=$(date +%F); echo "$now"
来源：http://hz.zdqjudy.top/gtgceckkdq.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtiiubtznj.html

echo $((1 + 2 * 3))
来源：http://hz.cheryme.top/gtkkvevqoc.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtiyzgbwjv.html

echo "scale=2; 10/3" | bc
来源：http://hz.hfpthk.cn/gtpuxadcbf.html

[R29] 定义函数
来源：http://hz.quarkkingdee.top/gtwxqnghdz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenjidiqi.icu/gtwctxyxrm.html

[R30] 函数返回状态码
来源：http://hz.shuidangran.top/gtzpkqcdfk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yangfankeji.com/gtnyudmnxk.html

[R31] 局部变量
来源：http://hz.hnqzz.top/gteimqbfwz.html

f() { local x=1; echo "$x"; }
来源：http://hz.aizwys.cn/gtyrzleffh.html

[R32] 参数个数校验
来源：http://hz.hnxiangtu.top/gtmsskmnip.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cheryme.top/gtyffxftzl.html

[R33] 捕获错误并提示行号
来源：http://hz.c1oappe.top/gtgfqcfzgf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yuanzhike.top/gtdtqhfvvd.html

[R34] 退出时清理
来源：http://hz.daria6918.cn/gtafxjmbqb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuetiantiany.cn/gttjyycjeh.html

[R35] 后台执行并等待
来源：http://hz.hongshengwenyu.top/gtengncjug.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sxryk.cn/gtpkrdpczb.html

[R36] 并发执行多个任务
来源：http://hz.dianchejie.cn/gtycgnugyn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj202588.top/gtdbxvvziq.html

[R37] 把输出赋给变量
来源：http://hz.yanxiufei.cn/gtusdrzvjk.html

files=$(ls -1)
来源：http://hz.sweek.top/gtrfovfkdw.html

[R38] 管道串联
来源：http://hz.316326.xyz/gtrlqelnwz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtplpkimec.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gtatfqgmfy.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtsebnfbjh.html

[R40] 追加写日志
来源：http://hz.gotoacloud.top/gtzqsxwvkw.html

echo "log" >> out.log
来源：http://hz.yueranfly.top/gteqomlzgh.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtkavyspdo.html

cmd >/dev/null 2>&1
来源：http://hz.zhengqikj.top/gtcsjzilht.html

[R42] 输入重定向
来源：http://hz.xuanzx.com/gtshxcqlsc.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtymadshxg.html

[R43] 按名字查找文件
来源：http://hz.zhijiandao.cn/gtpyxgkkow.html

find . -name "*.log" -type f
来源：http://hz.0kj1m.cn/gttbpkgyvy.html

[R44] 按修改时间查找
来源：http://hz.dianchejie.cn/gtozzrhisd.html

find . -mtime -7 -type f
来源：http://hz.9152youxi.cn/gtrjwmgrsi.html

[R45] 批量删除
来源：http://hz.shangyingyoupin.top/gtmwuxplcd.html

find . -name "*.tmp" -delete
来源：http://hz.hammf.cn/gtjwoimwhh.html

[R46] 递归替换文件内容
来源：http://hz.shuidangran.top/gtxkgdcihg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.quarkkingdee.top/gtzyorciwk.html

[R47] sed 单行替换
来源：http://hz.smart0.xyz/gtqegiwjtz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jianghu66.top/gtydgjdexl.html

[R48] awk 取指定列
来源：http://hz.yuanzhike.top/gtocdxvfjg.html

awk '{print $1, $3}' a.txt
来源：http://hz.pycfn.com/gtcsntrfwa.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtnlfthmgs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.feifeiyinyue.top/gtrrpaoaoz.html

[R50] awk 求和
来源：http://hz.tian-w.cn/gtwrlzqgqh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhixingplan.top/gtafidjpix.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gtcixygpoo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinyuanbaomall.cn/gtylxddxqg.html

[R52] 统计行数
来源：http://hz.wangdashe.top/gtmgsqubpr.html

wc -l a.txt
来源：http://hz.jyoumei.cn/gtymuyygjb.html

[R53] 查看文件头与实时尾
来源：http://hz.quarkkingdee.top/gtpsaxzbah.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.kuanghao11.cn/gtacwhhikv.html

[R54] 比较两个文件
来源：http://hz.jqgfzy.top/gtdkfmanwg.html

diff a.txt b.txt
来源：http://hz.yueranfly.top/gtsyuuxgwj.html

[R55] 压缩与解压
来源：http://hz.tian-w.cn/gtdukporld.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cheryme.top/gtxjkoxkax.html

[R56] 远程拷贝
来源：http://hz.gaohongyu789.top/gtikmyedkm.html

scp file user@host:/path/
来源：http://hz.shanyushiyangtech.top/gtpvzagpwm.html

[R57] 远程执行命令
来源：http://hz.cucudq.cn/gtdwhtrbtp.html

ssh user@host 'uptime'
来源：http://hz.9152youxi.cn/gtifuicwbv.html

[R58] 下载文件
来源：http://hz.dashuyun.cn/gtwsldtdkg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gtjphrpizp.html

[R59] 发 POST JSON
来源：http://hz.ydzc1.top/gtfapqqsxa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtisnwnlgo.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gttrkedmju.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxinkj.top/gtmhfwehub.html

[R61] 磁盘占用
来源：http://hz.gotoacloud.top/gtqdkirgby.html

df -h;  du -sh *
来源：http://hz.hongshengwenyu.top/gtlittcwbe.html

[R62] 找最占空间的文件
来源：http://hz.yj20258888.top/gtsmdopcqs.html

du -ah . | sort -rh | head -10
来源：http://hz.wangshuangyany.cn/gtytxisnyl.html

[R63] 内存与进程
来源：http://hz.svipenyu.cn/gtgvkhfzqg.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgufenzy.top/gtixjfncph.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtevqewjqi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhongyouzk.top/gtojeczdyx.html

[R65] 查看端口占用
来源：http://hz.aibaodan.cn/gtgknozqvd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.svipenyu.cn/gtrsydrpct.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtythakqob.html

crontab -e;  crontab -l
来源：http://hz.zhiwuduotai.top/gtvglqjvcr.html

[R67] 生成随机十六进制串
来源：http://hz.yuanzhike.top/gtjhtgtlrf.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gthhsbftdq.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtddvuvlao.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtchndingp.html

[R69] 生成随机密码
来源：http://hz.yuanzhike.top/gtvdlwtsoq.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuxming.cn/gtoonzeman.html

[R70] 时间戳与互转
来源：http://hz.yuxming.cn/gthzfhpaev.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gtvrwehpxc.html

[R71] 日期格式化
来源：http://hz.shuidangran.top/gtdwsdljlv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.9152youxi.cn/gtmwmaebws.html

[R72] 等待端口就绪
来源：http://hz.quarkkingdee.top/gtrnthivvh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtoanhotka.html

[R73] 分割大日志
来源：http://hz.jqgufenzy.top/gtqzfmwwuh.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangtech.top/gtcjkzzfup.html

[R74] 批量重命名
来源：http://hz.shzxlz.cn/gtsarmepkl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hammf.cn/gtzufysyjd.html

[R75] 导出环境变量
来源：http://hz.feifeiyinyue.top/gtkdhhxkjt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgfzy.top/gtegucwaqg.html

[R76] 使用临时文件
来源：http://hz.mhx1999.top/gtuyfankwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtesasfxvb.html

[R77] 读取用户输入
来源：http://hz.gaohongyu789.top/gtkamezmoh.html

read -rp "请输入: " ans
来源：http://hz.ybcxt.top/gteyoodqpy.html

[R78] 交互式菜单
来源：http://hz.jqgfzy.top/gtsbtouaim.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.svipenyu.cn/gtwcphvtnd.html

[R79] 解析命令行选项
来源：http://hz.redwolf501.top/gtssifclmb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gtztseouky.html

[R80] 查看脚本执行耗时
来源：http://hz.xuetiantiany.cn/gttmujqkzx.html

time ./run.sh
来源：http://hz.sweek.top/gtjpqdoiaw.html

================================================================================
来源：http://hz.svipenyu.cn/gtxjxktudz.html

S. C / C++ 专题
来源：http://hz.guannengcc.top/gtjtjhpvdt.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdqtkkgdg.html

[S01] C：Hello World
来源：http://hz.gzhubu.top/gtlxrnzpnj.html

#include <stdio.h>
来源：http://hz.cheryme.top/gtywhexscc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.andypj.xyz/gtfuxbochn.html

[S02] C：变量与格式化输出
来源：http://hz.cdnleiting.top/gtbjtaibmn.html

int a = 10; printf("%d\n", a);
来源：http://hz.hammf.cn/gtyhvhekaj.html

[S03] C：读入整数
来源：http://hz.feifeiyinyue.top/gtayqdrhwh.html

int x; scanf("%d", &x);
来源：http://hz.gotoacloud.top/gtsdhfunkc.html

[S04] C：字符串复制
来源：http://hz.yj202588.top/gtjimedvkp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydzc1.top/gtkvrbdscz.html

[S05] C：字符串长度
来源：http://hz.xylfe.cn/gtbepyokmr.html

strlen(s)
来源：http://hz.shuidangran.top/gthrxwjpvt.html

[S06] C：字符串比较
来源：http://hz.nanxuanxn.top/gtfwfwnvgl.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtjanslnzk.html

[S07] C：数组遍历求和
来源：http://hz.guannengcc.top/gtfiqtaopp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xingfuxueyuan.xyz/gtapgtcgcz.html

[S08] C：动态内存分配与释放
来源：http://hz.ivvv.top/gtoqwevbyt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jlsjyb.cn/gtwyaxsuxv.html

[S09] C：结构体定义与初始化
来源：http://hz.shuidangran.top/gthhihyftf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.meibo888.top/gtaprtzlqn.html

[S10] C：指针与解引用
来源：http://hz.316326.xyz/gtkqmauzrc.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gtvkspazir.html

[S11] C：逐行读文件
来源：http://hz.pengpengdd.cyou/gterykwegd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.redwolf501.top/gtgfartjkg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jyoumei.cn/gtyzqfxgyq.html

fclose(f);
来源：http://hz.tanke756.top/gtcmqmgzva.html

[S12] C：写文件
来源：http://hz.zhongyouzk.top/gtcjiiuiwd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dianchejie.cn/gtrwdthnzw.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtxqatvqvn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sweek.top/gtpwbhwkqj.html

[S14] C：枚举
来源：http://hz.0kj1m.cn/gtddqdvrvp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gtbvdevpnv.html

[S15] C：类型转换
来源：http://hz.daria6918.cn/gtgtofuqir.html

(double) a / b
来源：http://hz.fengsongda.top/gtuakcgbxr.html

[S16] C：位操作置位
来源：http://hz.zhoulong.xyz/gtukmurwfa.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gtvycvjtrk.html

[S17] C：安全拼接字符串
来源：http://hz.jqgfzy.top/gtawgacsuc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenzaomai.com/gtwfylodtr.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gtqxsfwimy.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gtyrqmtkfq.html

[S19] C：快速排序
来源：http://hz.vqdsnc.cn/gtuemguudo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtrzrzxgga.html

[S20] C：二分查找
来源：http://hz.jinqigufen.top/gtfmnwkfga.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gtvkdstxmv.html

[S21] C：字符类别判断
来源：http://hz.hnqzz.top/gtzgdjiyzr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtlaramrns.html

[S22] C：字符串转数字
来源：http://hz.shuidangran.top/gtynvftsat.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gtzzgezdxv.html

[S23] C：随机数
来源：http://hz.mhx1999.top/gtvnndkqai.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cheryme.top/gtvcmmsnpz.html

[S24] C：获取本地时间
来源：http://hz.hnxiangtu.top/gttbdpfykw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dashuyun.cn/gtmbolfrgy.html

[S25] C：内存拷贝
来源：http://hz.ydjk.org.cn/gtxrkvudcb.html

memcpy(dst, src, n);
来源：http://hz.yanxiufei.cn/gtmjrbsnmh.html

[S26] C：内存清零
来源：http://hz.nwbrower.top/gtwnnonnjn.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtrdexiauj.html

[S27] C：定义常量
来源：http://hz.aizwys.cn/gtfrueqhof.html

const double PI = 3.14159;
来源：http://hz.gogol.net.cn/gtuumwglcm.html

[S28] C：静态变量
来源：http://hz.zdqjudy.top/gtqcxpzkcu.html

static int counter = 0;
来源：http://hz.zhixingplan.top/gtplilhrzj.html

[S29] C：变参函数
来源：http://hz.nwbrower.top/gtbqyslrhm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.feifeiyinyue.top/gtuqxckapn.html

[S30] C：头文件保护
来源：http://hz.sysykeji.top/gtgcfhcnjx.html

#ifndef X_H
来源：http://hz.gaohongyu789.top/gttkkgguuk.html

#define X_H
来源：http://hz.tanke756.top/gtqpjsvces.html

#endif
来源：http://hz.yvedp.cn/gtpmngkzmj.html

[S31] C++：Hello World
来源：http://hz.jiagoushi.top/gtyqboornp.html

#include <iostream>
来源：http://hz.shzxlz.cn/gtagtpsmwv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cashguo.top/gtvutkoilt.html

[S32] C++：字符串
来源：http://hz.jlsjyb.cn/gtvijzydeo.html

std::string s = "hi";  s += "!";
来源：http://hz.ppjwa.cn/gtcpyafbmm.html

[S33] C++：vector 增删
来源：http://hz.nanxuanxn.top/gtabqulbyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258.top/gtsdghtxxk.html

[S34] C++：遍历 vector
来源：http://hz.bjfxy.top/gtdvrokfdq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sysykeji.top/gtkftstqhd.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtymnovtuv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtjbrxyofk.html

[S36] C++：unordered_map
来源：http://hz.svipenyu.cn/gtxmdlchyk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtikvqpajr.html

[S37] C++：set
来源：http://hz.aibaodan.cn/gtertqqciu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gteluuuvbo.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtuggpffur.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gtmcbommuo.html

[S39] C++：自定义比较器排序
来源：http://hz.shangyingyoupin.top/gtlcnedcwo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtrlgdtvnf.html

[S40] C++：查找元素
来源：http://hz.tian-w.cn/gtmwdcdmya.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.havefunace.top/gtvtozoxmz.html

[S41] C++：类与构造函数
来源：http://hz.fzhhl.top/gtqndrhykj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtxrujwjxs.html

[S42] C++：继承与虚函数
来源：http://hz.vqdsnc.cn/gtupftwzra.html

class B : public Base { public: void f() override {} };
来源：http://hz.cucudq.cn/gtmqotlwpz.html

[S43] C++：智能指针
来源：http://hz.snrcjt.cn/gtsqatypik.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnqzz.top/gtnqtxajbe.html

[S44] C++：引用传参
来源：http://hz.jinghuilouyu.cn/gttxqebhde.html

void inc(int &x) { ++x; }
来源：http://hz.tianlin.xyz/gtfydccleo.html

[S45] C++：lambda
来源：http://hz.gzhubu.top/gtcthusgbg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtgbjfpasp.html

[S46] C++：函数模板
来源：http://hz.nwbrower.top/gtwhcqknnv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xingfuxueyuan.xyz/gtiiqpnbyq.html

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gtaxetpnuo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuetiantiany.cn/gtkuncovmy.html

[S48] C++：逐行读文件
来源：http://hz.wangshuangyany.cn/gtnzpycstw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtjxhianll.html

while (std::getline(in, line)) { }
来源：http://hz.gogol.net.cn/gtomtoymua.html

[S49] C++：写文件
来源：http://hz.xingfuxueyuan.xyz/gtewotuuvq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.birdmap.top/gtxsfxhgwq.html

[S50] C++：格式化数字
来源：http://hz.svipenyu.cn/gtdoxudfxn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sufxvd.cn/gtkbrmxylz.html

[S51] C++：显式类型转换
来源：http://hz.shuidangran.top/gtoevgqkfi.html

static_cast<double>(a) / b
来源：http://hz.fengsongda.top/gteqlfhosc.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gtnxzlsfll.html

int size() const noexcept { return n_; }
来源：http://hz.hysaishi.cn/gtdtayfoly.html

[S53] C++：移动语义
来源：http://hz.havefunace.top/gtcwnpwpog.html

std::vector<int> w = std::move(v);
来源：http://hz.zhixingplan.top/gtmadraltf.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtfbksyvxr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jiagoushi.top/gtmbytcbop.html

[S55] C++：结构化绑定
来源：http://hz.yuanzhike.top/gtlezlepti.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.0kj1m.cn/gtpaxjwzzv.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtqyegirse.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgufenzy.top/gtdootaszm.html

[S57] C++：编译期常量
来源：http://hz.sufxvd.cn/gtvgcghrdf.html

constexpr int N = 10;
来源：http://hz.ivvv.top/gtzjlnvbry.html

[S58] C++：命名空间
来源：http://hz.gogol.net.cn/gtvffakvqc.html

namespace ns { int f() { return 1; } }
来源：http://hz.yangfankeji.com/gtnmzsktuy.html

[S59] C++：静态断言
来源：http://hz.jqgufenzy.top/gtbeyodehz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhaomingkeji.xyz/gttpghqlao.html

[S60] C++：遍历并删除元素
来源：http://hz.zdqjudy.top/gtprhxfjmr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtdxtyoaet.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbsdjfepm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinghuilouyu.cn/gtwklqbkqu.html

================================================================================
来源：http://hz.jlsjyb.cn/gtlihbfrzj.html

[T01] Kotlin：Hello World
来源：http://hz.shzxlz.cn/gtyvrjurje.html

println("Hello")
来源：http://hz.yvedp.cn/gtajhjtcmc.html

[T02] Kotlin：变量
来源：http://hz.dianchejie.cn/gtofzywqyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.9152youxi.cn/gtbhwqrjcl.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258888.top/gtojgylitc.html

"值: $b"
来源：http://hz.gzhubu.top/gtliokifry.html

[T04] Kotlin：空安全
来源：http://hz.sufxvd.cn/gtqbwvqpcb.html

val n: String? = null;  n?.length
来源：http://hz.yanxiufei.cn/gtdgacjnyc.html

[T05] Kotlin：when 表达式
来源：http://hz.zhaomingkeji.xyz/gtsbvlabst.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.smart0.xyz/gtapfkydvz.html

[T06] Kotlin：集合映射
来源：http://hz.svipenyu.cn/gtpjsdqvgq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cheryme.top/gtdtaotnuk.html


<!-- 参考信息 -->