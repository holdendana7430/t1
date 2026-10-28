代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shangyingyoupin.top/gtzfgktpty.html

[Q90] 生成序号列
来源：http://hz.hammf.cn/gtnmqjchyx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gtuvydkssv.html

================================================================================
来源：http://hz.9152youxi.cn/gtxdrwipwa.html

R. Bash 专题
来源：http://hz.pengpengdd.cyou/gtostvmrlu.html

================================================================================
来源：http://hz.hywenlv.cn/gtqwvjdjle.html

[R01] shebang 与严格模式
来源：http://hz.guowangkeji.top/gtfhqjlbmf.html

#!/usr/bin/env bash
来源：http://hz.snrcjt.cn/gtacoxsmli.html

set -euo pipefail
来源：http://hz.shangyingyoupin.top/gtmgqagura.html

[R02] 变量赋值与使用
来源：http://hz.cqqwz.cn/gttxrxxiwz.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gtmmnemqib.html

[R03] 只读变量
来源：http://hz.zhaomingkeji.xyz/gtsdosnkai.html

readonly PI=3.14
来源：http://hz.zhoulong.xyz/gtixiaebms.html

[R04] 位置参数
来源：http://hz.gaohongyu789.top/gtgbrodqfb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gtftjsqhok.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtmsbnadvm.html

name="${1:-default}"
来源：http://hz.snrcjt.cn/gtkoclwkwo.html

[R06] 判断命令是否存在
来源：http://hz.gaohongyu789.top/gtixhhhwuz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aibaodan.cn/gthyitynii.html

[R07] if 判断文件
来源：http://hz.shzxlz.cn/gtkiwzrdcm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.iojbl.cn/gtwkuqaawm.html

[R08] 数值比较
来源：http://hz.jinghuilouyu.cn/gtdakjvvdn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzhubu.top/gtjgyqaiju.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtjtzjyjyf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cashguo.top/gtvlmgasut.html

[R10] 正则匹配
来源：http://hz.yuanzhike.top/gtzdbhghgp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuetiantiany.cn/gtnkvtmmpq.html

[R11] case 多分支
来源：http://hz.sxryk.cn/gtnslkqmru.html

case "$1" in
来源：http://hz.jqgfzy.top/gtvykxcdlw.html

start) echo "启动" ;;
来源：http://hz.zycfv.cn/gtdbxeqmrs.html

stop)  echo "停止" ;;
来源：http://hz.cheryme.top/gtxhrkagep.html

*)     echo "未知命令" ;;
来源：http://hz.hnqzz.top/gtuzrwpgjb.html

esac
来源：http://hz.zhongyouzk.top/gtyncsrifk.html

[R12] for 遍历文件
来源：http://hz.zhaomingkeji.xyz/gtqjeourcl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.0kj1m.cn/gtceetwpje.html

[R13] for 计数循环
来源：http://hz.zhengqikj.top/gtcomwukwd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.guannengcc.top/gtfniukuwq.html

[R14] C 风格 for
来源：http://hz.shuidangran.top/gtglkfptnp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guowangkeji.top/gtucxoypnl.html

[R15] while 逐行读文件
来源：http://hz.hywenlv.cn/gtejytqzoq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.9152youxi.cn/gtribottou.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gtndordagr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.0kj1m.cn/gtvflqsbbz.html

[R17] 数组定义与取值
来源：http://hz.havefunace.top/gtnjqipepu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yangfankeji.com/gtwakishye.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gtketunsqa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtoihkpmnc.html

[R19] 数组长度
来源：http://hz.zdqjudy.top/gtcrsfiskl.html

echo "${#arr[@]}"
来源：http://hz.zhaomingkeji.xyz/gtttbcercu.html

[R20] 关联数组（字典）
来源：http://hz.jlsjyb.cn/gtuietcsuk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nwbrower.top/gtlysjyguh.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtgreiitpn.html

echo "${#s}"
来源：http://hz.zhaomingkeji.xyz/gtsfvmmrjc.html

[R22] 截取子串
来源：http://hz.dashuyun.cn/gtkciasfbb.html

echo "${s:0:5}"
来源：http://hz.xingfuxueyuan.xyz/gtdngervcp.html

[R23] 字符串替换
来源：http://hz.snrcjt.cn/gtxesfbdcb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.feifeiyinyue.top/gtftcplipm.html

[R24] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtkctjzteq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhaomingkeji.xyz/gtomutxbje.html

[R25] 去后缀 / 去前缀
来源：http://hz.cdnleiting.top/gtqzxdbwkx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.svipenyu.cn/gtpegikiuv.html

[R26] 命令替换
来源：http://hz.gzhubu.top/gtinympveg.html

now=$(date +%F); echo "$now"
来源：http://hz.hnxiangtu.top/gtlpalkjpk.html

[R27] 算术展开
来源：http://hz.cdnleiting.top/gtzbqhbrcf.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtwkqyjtnn.html

[R28] 浮点运算
来源：http://hz.bjfxy.top/gtclevnood.html

echo "scale=2; 10/3" | bc
来源：http://hz.snrcjt.cn/gtwoqlstvx.html

[R29] 定义函数
来源：http://hz.jlsjyb.cn/gtlqdfcorr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gthlzzuxmm.html

[R30] 函数返回状态码
来源：http://hz.redwolf501.top/gtzixeebuc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ywan-chungtsiang.top/gtqhovvata.html

[R31] 局部变量
来源：http://hz.jiagoushi.top/gtzponosog.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnxiangtu.top/gtpncdkuof.html

[R32] 参数个数校验
来源：http://hz.zhixingplan.top/gtvlpipvla.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.meibo888.top/gtvetjfltp.html

[R33] 捕获错误并提示行号
来源：http://hz.meibo888.top/gtldkjpxnd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.316326.xyz/gtasqqrpes.html

[R34] 退出时清理
来源：http://hz.wangshuangyany.cn/gtspursfdc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtczraxrvw.html

[R35] 后台执行并等待
来源：http://hz.feifeiyinyue.top/gtbhywdbhc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.iojbl.cn/gtjglqrdwv.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtsxtpgnhk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.mhx1999.top/gtlcddzvln.html

[R37] 把输出赋给变量
来源：http://hz.vqdsnc.cn/gtcclywtsr.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gtzvrackmt.html

[R38] 管道串联
来源：http://hz.cucudq.cn/gthxpbotpk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.wangshuangyany.cn/gtiutvscbh.html

[R39] 重定向标准输出与错误
来源：http://hz.zhengqikj.top/gtfjibnwtb.html

cmd > out.log 2>&1
来源：http://hz.316326.xyz/gtqnczlguo.html

[R40] 追加写日志
来源：http://hz.quarkkingdee.top/gtttliotld.html

echo "log" >> out.log
来源：http://hz.daria6918.cn/gtjllwcoex.html

[R41] 丢弃输出
来源：http://hz.guowangkeji.top/gtxcnmnplp.html

cmd >/dev/null 2>&1
来源：http://hz.aizwys.cn/gtqmahrsyk.html

[R42] 输入重定向
来源：http://hz.0kj1m.cn/gthhzvxzod.html

wc -l < a.txt
来源：http://hz.ivvv.top/gtpatnyxle.html

[R43] 按名字查找文件
来源：http://hz.xziqi.cn/gtxwscdier.html

find . -name "*.log" -type f
来源：http://hz.316326.xyz/gtwpzplsep.html

[R44] 按修改时间查找
来源：http://hz.316326.xyz/gtgbpjlcmd.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangtech.top/gtwvghyvzl.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtvjacmtbr.html

find . -name "*.tmp" -delete
来源：http://hz.yuxming.cn/gtaxqzdvud.html

[R46] 递归替换文件内容
来源：http://hz.xingfuxueyuan.xyz/gtnbzfqohr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cqqwz.cn/gtdsmaldhy.html

[R47] sed 单行替换
来源：http://hz.hywenlv.cn/gticilbfcz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cdnleiting.top/gtqbfzrozx.html

[R48] awk 取指定列
来源：http://hz.xuanzx.com/gtsaatuhbt.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtdvrxljfe.html

[R49] awk 带条件
来源：http://hz.zycfv.cn/gtxvmbqyxp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yvedp.cn/gtkzevlspa.html

[R50] awk 求和
来源：http://hz.316326.xyz/gthczbhdle.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yueranfly.top/gtopzndpej.html

[R51] 排序去重取前几
来源：http://hz.daxiang520.top/gtctrsgony.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinghuilouyu.cn/gtrpfqzcxv.html

[R52] 统计行数
来源：http://hz.52xcode.cn/gtgnyxdeni.html

wc -l a.txt
来源：http://hz.yj202588.top/gtwfwiqkjv.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtlcrghepm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenlongwang.top/gtewfbback.html

[R54] 比较两个文件
来源：http://hz.guannengcc.top/gtquyzgfea.html

diff a.txt b.txt
来源：http://hz.tian-w.cn/gtlzojulzl.html

[R55] 压缩与解压
来源：http://hz.ivvv.top/gtjplgthep.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangdashe.top/gttbqaxeal.html

[R56] 远程拷贝
来源：http://hz.svipenyu.cn/gtamutqoxg.html

scp file user@host:/path/
来源：http://hz.hnxiangtu.top/gtvbqkckvx.html

[R57] 远程执行命令
来源：http://hz.shuidangran.top/gtrutqbrks.html

ssh user@host 'uptime'
来源：http://hz.meibo888.top/gthsptznje.html

[R58] 下载文件
来源：http://hz.pengpengdd.cyou/gtntqxfclb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.feifeiyinyue.top/gttdgpoowd.html

[R59] 发 POST JSON
来源：http://hz.cucudq.cn/gtwwykvpas.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.vqdsnc.cn/gtqafxnwpb.html

[R60] 只看 HTTP 状态码
来源：http://hz.yongpay.top/gtqqnixtqr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gtmxihggvs.html

[R61] 磁盘占用
来源：http://hz.ydzc1.top/gtedyjpgzy.html

df -h;  du -sh *
来源：http://hz.nanxuanxn.top/gtnpgpwxmf.html

[R62] 找最占空间的文件
来源：http://hz.hywenlv.cn/gtgskrsywh.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtholejcrt.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtuhfzfvth.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtycrvjgni.html

[R64] 结束进程
来源：http://hz.shanyushiyangtech.top/gtovmtsgev.html

kill -9 $(pgrep -f app.py)
来源：http://hz.mhx1999.top/gtkcyaawvs.html

[R65] 查看端口占用
来源：http://hz.quarkkingdee.top/gtfjuudlvi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydzc1.top/gtnyrjndvj.html

[R66] 定时任务
来源：http://hz.yuxming.cn/gtcpxvipgc.html

crontab -e;  crontab -l
来源：http://hz.gzhubu.top/gttdwkuqlq.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtrjbxwwrw.html

openssl rand -hex 16
来源：http://hz.shuidangran.top/gtdoqggsyy.html

[R68] 计算文件校验值
来源：http://hz.yanxiufei.cn/gtmhncrkxq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuxming.cn/gtlxnzyxbw.html

[R69] 生成随机密码
来源：http://hz.pengpengdd.cyou/gtiuoxgpty.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtihskqami.html

[R70] 时间戳与互转
来源：http://hz.jyoumei.cn/gtwtjhwlxp.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtkfxlzmuh.html

[R71] 日期格式化
来源：http://hz.jqgufenzy.top/gtuhhdlgpy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xylfe.cn/gtlrljtqgv.html

[R72] 等待端口就绪
来源：http://hz.cheryme.top/gtaldcfdyh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtklbnxqgr.html

[R73] 分割大日志
来源：http://hz.birdmap.top/gtmcsrkhpz.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtmxzjoyal.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtrlmhtfvb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shuidangran.top/gturqhwmef.html

[R75] 导出环境变量
来源：http://hz.jinqigfzy.top/gtsclqbglv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.meibo888.top/gtfulnauvp.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtwsqktyun.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtfnngqhmf.html

[R77] 读取用户输入
来源：http://hz.sysykeji.top/gtmyuwfrpl.html

read -rp "请输入: " ans
来源：http://hz.gzhubu.top/gtphfzrjbl.html

[R78] 交互式菜单
来源：http://hz.jqgufenzy.top/gtcxxkzerx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenlongwang.top/gtropftoso.html

[R79] 解析命令行选项
来源：http://hz.yuanzhike.top/gthkctguay.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sysykeji.top/gtygpmkmeq.html

[R80] 查看脚本执行耗时
来源：http://hz.tian-w.cn/gtppzuoost.html

time ./run.sh
来源：http://hz.daria6918.cn/gtqkiuzcmy.html

================================================================================
来源：http://hz.xinyue.icu/gtqnghscnx.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtpyqmfvrw.html

================================================================================
来源：http://hz.sufxvd.cn/gtltbuhawb.html

[S01] C：Hello World
来源：http://hz.cucudq.cn/gtnkucfqhf.html

#include <stdio.h>
来源：http://hz.chenzaomai.com/gtemgrrrmu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.meibo888.top/gtfdetflcr.html

[S02] C：变量与格式化输出
来源：http://hz.pengpengdd.cyou/gtwrrnoxux.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtbvrthjxq.html

[S03] C：读入整数
来源：http://hz.shangyingyoupin.top/gtpyfamjcv.html

int x; scanf("%d", &x);
来源：http://hz.yj202588.top/gtzhdppmnk.html

[S04] C：字符串复制
来源：http://hz.jinqigufen.top/gtulmkchgy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.0kj1m.cn/gtmlhodmpu.html

[S05] C：字符串长度
来源：http://hz.jlsjyb.cn/gtqwatalig.html

strlen(s)
来源：http://hz.cashguo.top/gttvqegqzh.html

[S06] C：字符串比较
来源：http://hz.sxryk.cn/gtpnsqxceo.html

strcmp(a, b) == 0
来源：http://hz.cqqwz.cn/gtrzslrhuh.html

[S07] C：数组遍历求和
来源：http://hz.smart0.xyz/gtvatvnilt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangdashe.top/gtwqppokep.html

[S08] C：动态内存分配与释放
来源：http://hz.cheryme.top/gtlqzwhrbd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jlsjyb.cn/gtgokzohxs.html

[S09] C：结构体定义与初始化
来源：http://hz.iojbl.cn/gtelmlmeku.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj202588.top/gtabnpdjbo.html

[S10] C：指针与解引用
来源：http://hz.zhiwuduotai.top/gtuotghujs.html

int *p = &a;  *p = 5;
来源：http://hz.yangfankeji.com/gtvxtbdnah.html

[S11] C：逐行读文件
来源：http://hz.fengsongda.top/gtflllkibr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtfenxnrps.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuanzx.com/gtplmimqja.html

fclose(f);
来源：http://hz.52xcode.cn/gtboxkgpfu.html

[S12] C：写文件
来源：http://hz.yueranfly.top/gtchphrdtq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sysykeji.top/gtyodeiaxo.html

[S13] C：宏定义
来源：http://hz.jiagoushi.top/gtsgiqzhfr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuxming.cn/gtqnzxagtp.html

[S14] C：枚举
来源：http://hz.shanyushiyangtech.top/gtodjkedkr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cqqwz.cn/gtwedaskfh.html

[S15] C：类型转换
来源：http://hz.chenlongwang.top/gttottiedk.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtfjwsrnqa.html

[S16] C：位操作置位
来源：http://hz.tanke756.top/gthwgdwnhk.html

x |= (1 << 3);
来源：http://hz.hfpthk.cn/gtovokxdpe.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtoostsact.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtchzhzulg.html

[S18] C：命令行参数
来源：http://hz.tianlin.xyz/gtegtksjwl.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtqmhogzjs.html

[S19] C：快速排序
来源：http://hz.iojbl.cn/gtqbcjrrva.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.snrcjt.cn/gtqhogzgde.html

[S20] C：二分查找
来源：http://hz.andypj.xyz/gtkxyhrrps.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtdfskmgbu.html

[S21] C：字符类别判断
来源：http://hz.nanxuanxn.top/gtqlctzvkg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daxiang520.top/gtqgkwdaic.html

[S22] C：字符串转数字
来源：http://hz.yongpay.top/gtexvskhvr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hnqzz.top/gtpauglmpc.html

[S23] C：随机数
来源：http://hz.nanxinkj.top/gtzwywaxge.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sxryk.cn/gtxmynfktk.html

[S24] C：获取本地时间
来源：http://hz.jlsjyb.cn/gtysifhexm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zycfv.cn/gtjmbghbro.html

[S25] C：内存拷贝
来源：http://hz.yanxiufei.cn/gtsxnjdvkm.html

memcpy(dst, src, n);
来源：http://hz.ydzc1.top/gtcltbxpqg.html

[S26] C：内存清零
来源：http://hz.jinghuilouyu.cn/gtgdfjyrgw.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigufen.top/gtecsleucc.html

[S27] C：定义常量
来源：http://hz.c1oappe.top/gtcnpsscnn.html

const double PI = 3.14159;
来源：http://hz.yangfankeji.com/gtjnzziaan.html

[S28] C：静态变量
来源：http://hz.jinqigufen.top/gtegrlpsws.html

static int counter = 0;
来源：http://hz.ivvv.top/gtdrjrswtf.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gtekoouspo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.bjfxy.top/gtukneqsrw.html

[S30] C：头文件保护
来源：http://hz.wangshuangyany.cn/gtxwicdbri.html

#ifndef X_H
来源：http://hz.jinyuanbaomall.cn/gtmyebhnnu.html

#define X_H
来源：http://hz.ehwqpu.com/gtwvzqnrdq.html

#endif
来源：http://hz.sufxvd.cn/gtmmicakhp.html

[S31] C++：Hello World
来源：http://hz.dashuyun.cn/gtacrvxans.html

#include <iostream>
来源：http://hz.pengpengdd.cyou/gtuaegjxss.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuanzhike.top/gtxfmxlyac.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtsipygrvj.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gtseodhyyq.html

[S33] C++：vector 增删
来源：http://hz.yvedp.cn/gtrcfavsln.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gotoacloud.top/gtncxsmbcy.html

[S34] C++：遍历 vector
来源：http://hz.yanxiufei.cn/gtlalcmlqv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenzaomai.com/gtkycfzesk.html

[S35] C++：map
来源：http://hz.yvedp.cn/gtpsgyhphx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guowangkeji.top/gthliykvki.html

[S36] C++：unordered_map
来源：http://hz.gogol.net.cn/gtrjnshcmg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtcjjcdxai.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtpnhdtjdf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtlxymrpry.html

[S38] C++：排序
来源：http://hz.jqgfzy.top/gtjklxiuqg.html

std::sort(v.begin(), v.end());
来源：http://hz.0kj1m.cn/gterrdfary.html

[S39] C++：自定义比较器排序
来源：http://hz.c1oappe.top/gtkoawllrv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenlongwang.top/gteyavxcmp.html

[S40] C++：查找元素
来源：http://hz.zdqjudy.top/gtwzxkstbk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuanzhike.top/gtqxfyifsi.html

[S41] C++：类与构造函数
来源：http://hz.xuanzx.com/gtqpcwwtch.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hfpthk.cn/gtgddggabl.html

[S42] C++：继承与虚函数
来源：http://hz.jiagoushi.top/gtmxxzgihj.html

class B : public Base { public: void f() override {} };
来源：http://hz.meibo888.top/gtmdfipvzs.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gteolarkrc.html

auto p = std::make_unique<int>(5);
来源：http://hz.iojbl.cn/gtlhmevqtf.html

[S44] C++：引用传参
来源：http://hz.0kj1m.cn/gtmdxqfvtp.html

void inc(int &x) { ++x; }
来源：http://hz.shangyingyoupin.top/gttkwjfpqg.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gtwutqocjf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.meibo888.top/gtojphtxdp.html

[S46] C++：函数模板
来源：http://hz.xylfe.cn/gtbquhzvts.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.snrcjt.cn/gtscsdocns.html

[S47] C++：结构化绑定遍历
来源：http://hz.snrcjt.cn/gtorgkurkr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhaomingkeji.xyz/gtxmoyoqxm.html

[S48] C++：逐行读文件
来源：http://hz.cucudq.cn/gtkfpddfiv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtxsgirehk.html

while (std::getline(in, line)) { }
来源：http://hz.9152youxi.cn/gtezrgyolv.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtfbktkrvw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenlongwang.top/gtnbnvbrci.html

[S50] C++：格式化数字
来源：http://hz.fengsongda.top/gtjzdqrpdf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gtwnjnniwr.html

[S51] C++：显式类型转换
来源：http://hz.fengsongda.top/gtkgrvauxi.html

static_cast<double>(a) / b
来源：http://hz.gaohongyu789.top/gtncgvtwln.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtwqpbonut.html

int size() const noexcept { return n_; }
来源：http://hz.xinyue.icu/gtrukbsjxm.html

[S53] C++：移动语义
来源：http://hz.cucudq.cn/gtbhguuxvq.html

std::vector<int> w = std::move(v);
来源：http://hz.cucudq.cn/gtpcfvyund.html

[S54] C++：异常处理
来源：http://hz.yongpay.top/gthsymkeeh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shuidangran.top/gtatmcrlhj.html

[S55] C++：结构化绑定
来源：http://hz.zhoulong.xyz/gtljbzqtyb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ydjk.org.cn/gtoxclpjnw.html

[S56] C++：optional
来源：http://hz.ivvv.top/gtiebwolpp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgufenzy.top/gtejivhkgv.html

[S57] C++：编译期常量
来源：http://hz.vqdsnc.cn/gtsztqduzu.html

constexpr int N = 10;
来源：http://hz.snrcjt.cn/gtgceefcts.html

[S58] C++：命名空间
来源：http://hz.c1oappe.top/gthiewcdcf.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtbvlucdbv.html

[S59] C++：静态断言
来源：http://hz.yj20258888.top/gtpfsctszk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.0kj1m.cn/gtkkyvyvdk.html

[S60] C++：遍历并删除元素
来源：http://hz.fzhhl.top/gtlolnxmfa.html


<!-- 参考信息 -->