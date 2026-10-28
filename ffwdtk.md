代发 wailian999

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtqhhkfuqf.html

[R04] 位置参数
来源：http://hz.feifeiyinyue.top/gtkmozqjks.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tanke756.top/gtdaujuqqa.html

[R05] 参数默认值
来源：http://hz.chenlongwang.top/gtejogggdo.html

name="${1:-default}"
来源：http://hz.quarkkingdee.top/gtjnfszfbg.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtpwhkwsfs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daxiang520.top/gtkozbnpmb.html

[R07] if 判断文件
来源：http://hz.aizwys.cn/gtegkcmoqr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxinkj.top/gtaxeckmag.html

[R08] 数值比较
来源：http://hz.shzxlz.cn/gtilzhbfqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pycfn.com/gtepjelsrp.html

[R09] 字符串比较
来源：http://hz.snrcjt.cn/gthyhijszf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.smart0.xyz/gtxvyhogej.html

[R10] 正则匹配
来源：http://hz.zhijiandao.cn/gtgcignyin.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gthgikisab.html

[R11] case 多分支
来源：http://hz.haohaochexian.top/gtqshjsamv.html

case "$1" in
来源：http://hz.xylfe.cn/gtmvhoxxwh.html

start) echo "启动" ;;
来源：http://hz.dashuyun.cn/gtctsocyso.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtsvtaqciz.html

*)     echo "未知命令" ;;
来源：http://hz.nanxuanxn.top/gteashuuqg.html

esac
来源：http://hz.tanke756.top/gtrxrxpfwz.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gthncxbtqy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.redwolf501.top/gtookgusov.html

[R13] for 计数循环
来源：http://hz.hywenlv.cn/gtyrlcxgoi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pycfn.com/gtdifsfakm.html

[R14] C 风格 for
来源：http://hz.yueranfly.top/gtxdfdlhcz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guannengcc.top/gtpaqoxbbb.html

[R15] while 逐行读文件
来源：http://hz.havefunace.top/gtzvszytlk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nwbrower.top/gtsqbifwxx.html

[R16] until 等待条件
来源：http://hz.ehwqpu.com/gtmcisqgvi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtavoxyjtk.html

[R17] 数组定义与取值
来源：http://hz.jlsjyb.cn/gtfchpwqct.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tianlin.xyz/gtxsrgbcup.html

[R18] 遍历数组
来源：http://hz.cqqwz.cn/gtcxsocodt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtznrotvnq.html

[R19] 数组长度
来源：http://hz.tian-w.cn/gthxyikoac.html

echo "${#arr[@]}"
来源：http://hz.zhengqikj.top/gtyipfnmqq.html

[R20] 关联数组（字典）
来源：http://hz.hongshengwenyu.top/gtroskueri.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jqgufenzy.top/gtfadyufwb.html

[R21] 字符串长度
来源：http://hz.zhijiandao.cn/gtlrfxsbtu.html

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtvhjzzlms.html

[R22] 截取子串
来源：http://hz.iojbl.cn/gtetxgvtjo.html

echo "${s:0:5}"
来源：http://hz.c1oappe.top/gtujhyekxf.html

[R23] 字符串替换
来源：http://hz.guannengcc.top/gtqhbxuoby.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ybcxt.top/gtrqzaflhh.html

[R24] 大小写转换
来源：http://hz.yueranfly.top/gtqlkxfnuz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hammf.cn/gtvllrhhim.html

[R25] 去后缀 / 去前缀
来源：http://hz.haohaochexian.top/gtqdtlcfds.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yonumen.top/gtwtvqlqad.html

[R26] 命令替换
来源：http://hz.zhongyouzk.top/gtqbbfymia.html

now=$(date +%F); echo "$now"
来源：http://hz.jiagoushi.top/gtpkpwzfgn.html

[R27] 算术展开
来源：http://hz.daria6918.cn/gtuxahlbac.html

echo $((1 + 2 * 3))
来源：http://hz.nwbrower.top/gtrggmcejp.html

[R28] 浮点运算
来源：http://hz.316326.xyz/gtuesaumkf.html

echo "scale=2; 10/3" | bc
来源：http://hz.gzhubu.top/gtkgjkxeqc.html

[R29] 定义函数
来源：http://hz.zhijiandao.cn/gttxhbmble.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtdsbdujdz.html

[R30] 函数返回状态码
来源：http://hz.ybcxt.top/gtzeetothg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gthynjzvli.html

[R31] 局部变量
来源：http://hz.vqdsnc.cn/gthivyhkmc.html

f() { local x=1; echo "$x"; }
来源：http://hz.mhx1999.top/gtexhrtvwt.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtuamxjdkb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtzgjmojtx.html

[R33] 捕获错误并提示行号
来源：http://hz.dianchejie.cn/gtdynutkfn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xylfe.cn/gtdljebvvk.html

[R34] 退出时清理
来源：http://hz.zhijiandao.cn/gttcfhnavj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtfsgstobd.html

[R35] 后台执行并等待
来源：http://hz.cheryme.top/gtpojhxoao.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ivvv.top/gtigljcpke.html

[R36] 并发执行多个任务
来源：http://hz.yvedp.cn/gtnopwajkn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gtirkqxjwd.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gtaznndvbj.html

files=$(ls -1)
来源：http://hz.fengsongda.top/gtdhzadskz.html

[R38] 管道串联
来源：http://hz.hfpthk.cn/gtvmeudzdm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cheryme.top/gtrfoqcioe.html

[R39] 重定向标准输出与错误
来源：http://hz.jyoumei.cn/gttdxuuvjj.html

cmd > out.log 2>&1
来源：http://hz.yj202588.top/gthlwtanxe.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gthmdfsxrr.html

echo "log" >> out.log
来源：http://hz.xuetiantiany.cn/gtotacfpcm.html

[R41] 丢弃输出
来源：http://hz.jiagoushi.top/gtfkiauqyb.html

cmd >/dev/null 2>&1
来源：http://hz.0kj1m.cn/gtrpwknrsr.html

[R42] 输入重定向
来源：http://hz.jinqigufen.top/gtrthhyjmk.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtrozjxxtz.html

[R43] 按名字查找文件
来源：http://hz.wangdashe.top/gtwsijwlob.html

find . -name "*.log" -type f
来源：http://hz.jqgufenzy.top/gtlrhchabq.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtzebynkgp.html

find . -mtime -7 -type f
来源：http://hz.jinqigfzy.top/gtmptcsqah.html

[R45] 批量删除
来源：http://hz.jinqigufen.top/gtxronshxl.html

find . -name "*.tmp" -delete
来源：http://hz.hywenlv.cn/gtocvhsvot.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gtoxtddzoe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.redwolf501.top/gtevnqsssy.html

[R47] sed 单行替换
来源：http://hz.sufxvd.cn/gtzszzpudm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258888.top/gthlatqstb.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtqwnrazil.html

awk '{print $1, $3}' a.txt
来源：http://hz.smart0.xyz/gtuyaolfdn.html

[R49] awk 带条件
来源：http://hz.jlsjyb.cn/gtdxskvosd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hfpthk.cn/gthyehezbe.html

[R50] awk 求和
来源：http://hz.yonumen.top/gtvqebwkod.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhongyouzk.top/gtsoyessqb.html

[R51] 排序去重取前几
来源：http://hz.ivvv.top/gtojpohseb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hongshengwenyu.top/gtpkdvhnnp.html

[R52] 统计行数
来源：http://hz.iojbl.cn/gtrorhlzvs.html

wc -l a.txt
来源：http://hz.hnqzz.top/gtbjdfyzpg.html

[R53] 查看文件头与实时尾
来源：http://hz.xuetiantiany.cn/gtagblimoi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gtprbyzfua.html

[R54] 比较两个文件
来源：http://hz.ydzc1.top/gtsciwhowr.html

diff a.txt b.txt
来源：http://hz.cucudq.cn/gttmvfzilp.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gtypqzuaxc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shzxlz.cn/gtnycqoxbg.html

[R56] 远程拷贝
来源：http://hz.yueranfly.top/gtvikqiyyf.html

scp file user@host:/path/
来源：http://hz.gzhubu.top/gthvbxhqmo.html

[R57] 远程执行命令
来源：http://hz.wangdashe.top/gtzfjsxvcp.html

ssh user@host 'uptime'
来源：http://hz.jinghuilouyu.cn/gtvphhynce.html

[R58] 下载文件
来源：http://hz.birdmap.top/gtmhbqgywx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtsknjwyej.html

[R59] 发 POST JSON
来源：http://hz.xinyue.icu/gtvobeakex.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tanke756.top/gtwmxbzpeh.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuanzx.com/gtpdzgkscr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hongshengwenyu.top/gtgdzkyqwm.html

[R61] 磁盘占用
来源：http://hz.yvedp.cn/gtrdowjhcv.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtaveazief.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gtmzjspyep.html

du -ah . | sort -rh | head -10
来源：http://hz.hfpthk.cn/gtjupekuxl.html

[R63] 内存与进程
来源：http://hz.tanke756.top/gttlzimrzy.html

free -h;  ps aux | grep nginx
来源：http://hz.wangdashe.top/gtdfrlqxtg.html

[R64] 结束进程
来源：http://hz.hywenlv.cn/gtcztjcchp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gzhubu.top/gtvunkkonz.html

[R65] 查看端口占用
来源：http://hz.daxiang520.top/gtzogtjywb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.haohaochexian.top/gtlgceyvmz.html

[R66] 定时任务
来源：http://hz.guowangkeji.top/gtajhqkvmh.html

crontab -e;  crontab -l
来源：http://hz.yongpay.top/gtggpihkfg.html

[R67] 生成随机十六进制串
来源：http://hz.sysykeji.top/gthxnxdrru.html

openssl rand -hex 16
来源：http://hz.kuanghao11.cn/gtzvctdnvc.html

[R68] 计算文件校验值
来源：http://hz.cdnleiting.top/gtnhgulxai.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tian-w.cn/gtlabcxhsg.html

[R69] 生成随机密码
来源：http://hz.jinyuanbaomall.cn/gtqhbqljmi.html

head -c 16 /dev/urandom | base64
来源：http://hz.bjfxy.top/gtyrumizfz.html

[R70] 时间戳与互转
来源：http://hz.tian-w.cn/gtiusqmxot.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigfzy.top/gtpqpktfbf.html

[R71] 日期格式化
来源：http://hz.fengsongda.top/gtbqlhxnht.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnxiangtu.top/gtycamrlfl.html

[R72] 等待端口就绪
来源：http://hz.zhaomingkeji.xyz/gtcuprxnoq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tianlin.xyz/gtylskzmdy.html

[R73] 分割大日志
来源：http://hz.0kj1m.cn/gtkqqixbwl.html

split -l 1000 big.log part_
来源：http://hz.hnxiangtu.top/gtmcydvapm.html

[R74] 批量重命名
来源：http://hz.yueranfly.top/gtuelpyoyu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shzxlz.cn/gtrdvcetcx.html

[R75] 导出环境变量
来源：http://hz.bjfxy.top/gthbaxepcr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tian-w.cn/gtbeqbcfha.html

[R76] 使用临时文件
来源：http://hz.jinghuilouyu.cn/gtwtqdenin.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtbkkaiqks.html

[R77] 读取用户输入
来源：http://hz.zhongyouzk.top/gtzebcugnv.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gtyuohtnxl.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtpznyvpcv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gtnfbbaxyc.html

[R79] 解析命令行选项
来源：http://hz.wangshuangyany.cn/gtvzzgofzu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cdnleiting.top/gtzphzkrhv.html

[R80] 查看脚本执行耗时
来源：http://hz.chenjidiqi.icu/gtbbnfdlnm.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtlkwjvyzn.html

================================================================================
来源：http://hz.sxryk.cn/gtqtppgetz.html

S. C / C++ 专题
来源：http://hz.ppjwa.cn/gtujgvzepe.html

================================================================================
来源：http://hz.svipenyu.cn/gtltdofiwc.html

[S01] C：Hello World
来源：http://hz.tian-w.cn/gtxzvxrild.html

#include <stdio.h>
来源：http://hz.nanxuanxn.top/gtdohsstrs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.andypj.xyz/gtrnkuvqfn.html

[S02] C：变量与格式化输出
来源：http://hz.sxryk.cn/gtnqqdgkjk.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gthvgsoijw.html

[S03] C：读入整数
来源：http://hz.sufxvd.cn/gtwfunroro.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gtzqacbztz.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtdltosflx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gtxiufzlnv.html

[S05] C：字符串长度
来源：http://hz.jinqigfzy.top/gtgqgftvwt.html

strlen(s)
来源：http://hz.mhx1999.top/gtymnnluwd.html

[S06] C：字符串比较
来源：http://hz.hfpthk.cn/gtsfzfyxsv.html

strcmp(a, b) == 0
来源：http://hz.hfpthk.cn/gtfwlghsjr.html

[S07] C：数组遍历求和
来源：http://hz.cashguo.top/gtsgbhxwpi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.vqdsnc.cn/gtfooeluwx.html

[S08] C：动态内存分配与释放
来源：http://hz.jlsjyb.cn/gtedgepmyn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ywan-chungtsiang.top/gttzuljyyu.html

[S09] C：结构体定义与初始化
来源：http://hz.zhixingplan.top/gtzgtarbyn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cqqwz.cn/gtjhhjkwme.html

[S10] C：指针与解引用
来源：http://hz.tanke756.top/gtlrppymeo.html

int *p = &a;  *p = 5;
来源：http://hz.chenjidiqi.icu/gtofzlvtkj.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtqbplyclc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.redwolf501.top/gtoxidmchk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtwpasmopy.html

fclose(f);
来源：http://hz.andypj.xyz/gtgqqzrjzb.html

[S12] C：写文件
来源：http://hz.nanxinkj.top/gtgocscdhz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhongyouzk.top/gttsnmfrhu.html

[S13] C：宏定义
来源：http://hz.vqdsnc.cn/gtixodokmu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tanke756.top/gtouwfkpzz.html

[S14] C：枚举
来源：http://hz.yvedp.cn/gtvtlodbjm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hammf.cn/gtpaucukfk.html

[S15] C：类型转换
来源：http://hz.meibo888.top/gtqsuifihm.html

(double) a / b
来源：http://hz.c1oappe.top/gtdhgffdky.html

[S16] C：位操作置位
来源：http://hz.ppjwa.cn/gtgbizkdst.html

x |= (1 << 3);
来源：http://hz.shuidangran.top/gteqemwxut.html

[S17] C：安全拼接字符串
来源：http://hz.yj202588.top/gtcngeezwr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxinkj.top/gtfhgcmnuh.html

[S18] C：命令行参数
来源：http://hz.xylfe.cn/gtqtoqtife.html

int main(int argc, char **argv)
来源：http://hz.0kj1m.cn/gtvvrvhwwn.html

[S19] C：快速排序
来源：http://hz.yvedp.cn/gtpuevflig.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtjfpdwldd.html

[S20] C：二分查找
来源：http://hz.jinqigfzy.top/gtjwahdfqm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gtunlufyok.html

[S21] C：字符类别判断
来源：http://hz.ivvv.top/gtmclzvsug.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ppjwa.cn/gtvpwaijqo.html

[S22] C：字符串转数字
来源：http://hz.xuanzx.com/gtwbsxcdas.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuanzhike.top/gtascicdvs.html

[S23] C：随机数
来源：http://hz.haohaochexian.top/gtwehmmrwg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtckglazaw.html

[S24] C：获取本地时间
来源：http://hz.9152youxi.cn/gtuvuhxpbq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenzaomai.com/gtsemhcegw.html

[S25] C：内存拷贝
来源：http://hz.xuanzx.com/gtogicxypm.html

memcpy(dst, src, n);
来源：http://hz.yongpay.top/gtekgqqvun.html

[S26] C：内存清零
来源：http://hz.zhaomingkeji.xyz/gtfddakiuk.html

memset(a, 0, sizeof a);
来源：http://hz.bjfxy.top/gtzkofsgbt.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtrbyzdgzn.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtbzclrbve.html

[S28] C：静态变量
来源：http://hz.shuidangran.top/gtdbplrpmu.html

static int counter = 0;
来源：http://hz.nanxuanxn.top/gtcrndtmek.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtzotxtyoz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hfpthk.cn/gtmcukgjyu.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtrhaorpyo.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtwmzbuldn.html

#define X_H
来源：http://hz.zhengqikj.top/gtatsmtctz.html

#endif
来源：http://hz.hongshengwenyu.top/gtjnluatav.html

[S31] C++：Hello World
来源：http://hz.zhongyouzk.top/gthhvsptlp.html

#include <iostream>
来源：http://hz.nwbrower.top/gtwlzypfyp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ydzc1.top/gthrughlps.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gthssigdxv.html

std::string s = "hi";  s += "!";
来源：http://hz.cdnleiting.top/gtkfzjlcxi.html

[S33] C++：vector 增删
来源：http://hz.yangfankeji.com/gtqlbgkruy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dianchejie.cn/gteeairzvy.html

[S34] C++：遍历 vector
来源：http://hz.yuxming.cn/gtwoxxihba.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ybcxt.top/gtfjoahzwf.html

[S35] C++：map
来源：http://hz.jyoumei.cn/gtotzvbrke.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yonumen.top/gtebpwzjzf.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gtfxbspkcz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gthtloyhyw.html

[S37] C++：set
来源：http://hz.zycfv.cn/gtahkydwtc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yueranfly.top/gtmnhethsx.html

[S38] C++：排序
来源：http://hz.shuidangran.top/gtiqeexito.html

std::sort(v.begin(), v.end());
来源：http://hz.jianghu66.top/gtycaahfqg.html

[S39] C++：自定义比较器排序
来源：http://hz.yueranfly.top/gtamsmyeno.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gtklamxkef.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gtmnrxkzuq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtlgmrhcdl.html

[S41] C++：类与构造函数
来源：http://hz.hongshengwenyu.top/gtypmfgxix.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dianchejie.cn/gtfgdbyarh.html

[S42] C++：继承与虚函数
来源：http://hz.wangdashe.top/gthemdnzws.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtqvwlcbhv.html

[S43] C++：智能指针
来源：http://hz.ydzc1.top/gtlokutarw.html

auto p = std::make_unique<int>(5);
来源：http://hz.shangyingyoupin.top/gtnrobplag.html

[S44] C++：引用传参
来源：http://hz.zhaomingkeji.xyz/gtnccnksop.html

void inc(int &x) { ++x; }
来源：http://hz.zhongyouzk.top/gtufhsimlu.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gtlunorwwj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shangyingyoupin.top/gthrvpkeqo.html

[S46] C++：函数模板
来源：http://hz.zhiwuduotai.top/gtvqpyztkr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.andypj.xyz/gttbqahbih.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gtqcfqawep.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sufxvd.cn/gtphllyxaq.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtbtartvhp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xylfe.cn/gtuslhwxwv.html

while (std::getline(in, line)) { }
来源：http://hz.yueranfly.top/gtdtxtlaje.html

[S49] C++：写文件
来源：http://hz.chenlongwang.top/gtjfrtngkt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.snrcjt.cn/gtoygrpddz.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtufakcbfz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydzc1.top/gtunqcnncv.html

[S51] C++：显式类型转换
来源：http://hz.zhiwuduotai.top/gttsqtvila.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangkeji.top/gtfhomptvz.html

[S52] C++：const 与 noexcept
来源：http://hz.9152youxi.cn/gtzlvleotu.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtjvzusiiy.html

[S53] C++：移动语义
来源：http://hz.nwbrower.top/gtwdzmgsxs.html

std::vector<int> w = std::move(v);
来源：http://hz.ywan-chungtsiang.top/gtrkhmghdw.html

[S54] C++：异常处理
来源：http://hz.hnxiangtu.top/gtxhutsvgx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydzc1.top/gtnhbdpkmq.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gtxrsrzfzi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.meibo888.top/gtaumatpdo.html

[S56] C++：optional
来源：http://hz.fzhhl.top/gtzjgsvcfj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sxryk.cn/gtcbfgnuak.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtskgqjtby.html

constexpr int N = 10;
来源：http://hz.hysaishi.cn/gtnfmizbxb.html

[S58] C++：命名空间
来源：http://hz.havefunace.top/gtwjaiavnf.html

namespace ns { int f() { return 1; } }
来源：http://hz.sufxvd.cn/gttjvvsgyr.html

[S59] C++：静态断言
来源：http://hz.ybcxt.top/gtwsupmlsm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nwbrower.top/gtthedpgxf.html

[S60] C++：遍历并删除元素
来源：http://hz.kuanghao11.cn/gtcbkzfmnq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tanke756.top/gtxixvhskg.html

================================================================================
来源：http://hz.0kj1m.cn/gttlhsrybb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtyxqizfii.html

================================================================================
来源：http://hz.smart0.xyz/gtfipzipwc.html

[T01] Kotlin：Hello World
来源：http://hz.jiagoushi.top/gtnhdktrdl.html

println("Hello")
来源：http://hz.jinqigufen.top/gtlztqzuri.html

[T02] Kotlin：变量
来源：http://hz.fzhhl.top/gtzybywoii.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.havefunace.top/gtxqoeprsp.html

[T03] Kotlin：字符串模板
来源：http://hz.sxryk.cn/gteskgisly.html

"值: $b"
来源：http://hz.pengpengdd.cyou/gtpgklcwbh.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtqfrakckd.html

val n: String? = null;  n?.length
来源：http://hz.vqdsnc.cn/gtgwxkvzzl.html


<!-- 参考信息 -->