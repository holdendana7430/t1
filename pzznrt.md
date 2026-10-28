代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.yueranfly.top/gtrplnaqjm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.birdmap.top/gttmpkbxat.html

[Q87] JSON 字段做条件
来源：http://hz.sufxvd.cn/gtlbeloiud.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shuidangran.top/gtkuyxqohc.html

[Q88] 行转列（条件聚合）
来源：http://hz.ivvv.top/gtbjalhegg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtkqrsvauz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sysykeji.top/gtaumddtrn.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gtvrybhmeq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xziqi.cn/gtygghcijr.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtjveysoyl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.svipenyu.cn/gtidsqruhw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtrvjptnvw.html

R. Bash 专题
来源：http://hz.cheryme.top/gtqpajazlh.html

================================================================================
来源：http://hz.jinqigufen.top/gtvndngkrn.html

[R01] shebang 与严格模式
来源：http://hz.xuetiantiany.cn/gtkjtqupnz.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gtdihlxttn.html

set -euo pipefail
来源：http://hz.zycfv.cn/gtagjpavdn.html

[R02] 变量赋值与使用
来源：http://hz.jqgufenzy.top/gtskslsgcs.html

name="Tom"; echo "$name"
来源：http://hz.nwbrower.top/gtgolzqjrn.html

[R03] 只读变量
来源：http://hz.xinyue.icu/gthkooqwnz.html

readonly PI=3.14
来源：http://hz.hnxiangtu.top/gtwmimwntl.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtsezjrmmz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gttzelcubk.html

[R05] 参数默认值
来源：http://hz.birdmap.top/gtaqavodzv.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtljbiqnpn.html

[R06] 判断命令是否存在
来源：http://hz.zhijiandao.cn/gtrrvansmz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nwbrower.top/gticbhkisy.html

[R07] if 判断文件
来源：http://hz.0kj1m.cn/gtgqnqmxpv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jianghu66.top/gtxjclrojp.html

[R08] 数值比较
来源：http://hz.jinghuilouyu.cn/gtmlhlaqlm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guowangkeji.top/gtejfosemn.html

[R09] 字符串比较
来源：http://hz.yuxming.cn/gtmvfzbqyh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinghuilouyu.cn/gtgipmloob.html

[R10] 正则匹配
来源：http://hz.guowangkeji.top/gtpjsfaljv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hammf.cn/gtczcygwvv.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gtbutcrspt.html

case "$1" in
来源：http://hz.haohaochexian.top/gtclvdmcvx.html

start) echo "启动" ;;
来源：http://hz.guowangkeji.top/gtwninuulb.html

stop)  echo "停止" ;;
来源：http://hz.chenzaomai.com/gtebwdngit.html

*)     echo "未知命令" ;;
来源：http://hz.yueranfly.top/gtgojtofde.html

esac
来源：http://hz.zhijiandao.cn/gtcatpsptz.html

[R12] for 遍历文件
来源：http://hz.zhoulong.xyz/gtogblsxqu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258888.top/gtvouqaqzl.html

[R13] for 计数循环
来源：http://hz.zhongyouzk.top/gtbwpbjbmg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gtdqvvqpsd.html

[R14] C 风格 for
来源：http://hz.hammf.cn/gtvfdutqtq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hammf.cn/gtsymainwq.html

[R15] while 逐行读文件
来源：http://hz.jqgfzy.top/gtqjnpfyrg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtqajgeeja.html

[R16] until 等待条件
来源：http://hz.sweek.top/gtexauzlad.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.haohaochexian.top/gtjsdofdap.html

[R17] 数组定义与取值
来源：http://hz.bjfxy.top/gtesduyjpr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aizwys.cn/gtyqzhmnex.html

[R18] 遍历数组
来源：http://hz.svipenyu.cn/gtrilflgpr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shangyingyoupin.top/gtjfbzddrt.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtxyprqxgj.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtjgjjoirn.html

[R20] 关联数组（字典）
来源：http://hz.smart0.xyz/gtylztkefm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gtlcvadzbf.html

[R21] 字符串长度
来源：http://hz.dashuyun.cn/gtnsxlyigl.html

echo "${#s}"
来源：http://hz.sweek.top/gtyrbrkhjq.html

[R22] 截取子串
来源：http://hz.xziqi.cn/gtkebbejgk.html

echo "${s:0:5}"
来源：http://hz.jqgfzy.top/gtcxjihccy.html

[R23] 字符串替换
来源：http://hz.gogol.net.cn/gtvutidppl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gtlxgkewhj.html

[R24] 大小写转换
来源：http://hz.chenzaomai.com/gtxfstlzlz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258.top/gtptfekkex.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhaomingkeji.xyz/gtdofmobhd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ivvv.top/gtnatryqut.html

[R26] 命令替换
来源：http://hz.andypj.xyz/gtsxazdwvr.html

now=$(date +%F); echo "$now"
来源：http://hz.aizwys.cn/gtdvnqkptn.html

[R27] 算术展开
来源：http://hz.feifeiyinyue.top/gtmhhdxtwj.html

echo $((1 + 2 * 3))
来源：http://hz.pycfn.com/gtzrjtutcn.html

[R28] 浮点运算
来源：http://hz.aizwys.cn/gtvkfoxdro.html

echo "scale=2; 10/3" | bc
来源：http://hz.c1oappe.top/gtjcetmitl.html

[R29] 定义函数
来源：http://hz.yvedp.cn/gtqqndrran.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.pengpengdd.cyou/gtuyameijz.html

[R30] 函数返回状态码
来源：http://hz.shuidangran.top/gtspauwosd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnxiangtu.top/gtfsfoeyhi.html

[R31] 局部变量
来源：http://hz.xuetiantiany.cn/gthwfkcoqm.html

f() { local x=1; echo "$x"; }
来源：http://hz.dianchejie.cn/gtfgbfjwvs.html

[R32] 参数个数校验
来源：http://hz.jiagoushi.top/gtyslnhyvv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.iojbl.cn/gtelikemaj.html

[R33] 捕获错误并提示行号
来源：http://hz.jianghu66.top/gtmoqspahm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenjidiqi.icu/gtvlaxapsd.html

[R34] 退出时清理
来源：http://hz.quarkkingdee.top/gtvuxdylvw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtyigbyaac.html

[R35] 后台执行并等待
来源：http://hz.daxiang520.top/gtpgcueopd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.smart0.xyz/gtklbdzbtc.html

[R36] 并发执行多个任务
来源：http://hz.iojbl.cn/gtgdvanrih.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gturdqylbq.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangkeji.top/gtkkwprryf.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gtmnnixexl.html

[R38] 管道串联
来源：http://hz.smart0.xyz/gtnrnggveo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hysaishi.cn/gttgrhxxov.html

[R39] 重定向标准输出与错误
来源：http://hz.xinyue.icu/gtfrupqrbp.html

cmd > out.log 2>&1
来源：http://hz.nanxinkj.top/gtzisxnlzf.html

[R40] 追加写日志
来源：http://hz.jinqigfzy.top/gtugaoqmrw.html

echo "log" >> out.log
来源：http://hz.jyoumei.cn/gttyadbslg.html

[R41] 丢弃输出
来源：http://hz.redwolf501.top/gthttirwxv.html

cmd >/dev/null 2>&1
来源：http://hz.yvedp.cn/gtucwfbxmc.html

[R42] 输入重定向
来源：http://hz.0kj1m.cn/gtvhpypqyy.html

wc -l < a.txt
来源：http://hz.cashguo.top/gtqwxsdjxg.html

[R43] 按名字查找文件
来源：http://hz.zhixingplan.top/gthgtuaigu.html

find . -name "*.log" -type f
来源：http://hz.jianghu66.top/gtudgyrgfo.html

[R44] 按修改时间查找
来源：http://hz.guannengcc.top/gttsxxuarg.html

find . -mtime -7 -type f
来源：http://hz.shzxlz.cn/gtsmpxfgoh.html

[R45] 批量删除
来源：http://hz.ydjk.org.cn/gtixkubxbv.html

find . -name "*.tmp" -delete
来源：http://hz.xylfe.cn/gtpnjmezoi.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangtech.top/gtuviejvci.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.haohaochexian.top/gtwqwxqmce.html

[R47] sed 单行替换
来源：http://hz.xingfuxueyuan.xyz/gtdoumsjsh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhengqikj.top/gtselxfhvq.html

[R48] awk 取指定列
来源：http://hz.dashuyun.cn/gtutqzgjrr.html

awk '{print $1, $3}' a.txt
来源：http://hz.hysaishi.cn/gtaoafshrq.html

[R49] awk 带条件
来源：http://hz.xingfuxueyuan.xyz/gtjbmlhbde.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gtnczvyiuy.html

[R50] awk 求和
来源：http://hz.hammf.cn/gtetmqmqgk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.bjfxy.top/gtktyzyiap.html

[R51] 排序去重取前几
来源：http://hz.jianghu66.top/gtwmpuyyha.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aizwys.cn/gtinlmwqtr.html

[R52] 统计行数
来源：http://hz.chenlongwang.top/gtcrohggso.html

wc -l a.txt
来源：http://hz.jinghuilouyu.cn/gtkusayvvw.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gtmdwykdpz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shzxlz.cn/gtdxxmlmti.html

[R54] 比较两个文件
来源：http://hz.cucudq.cn/gtsgeokxeh.html

diff a.txt b.txt
来源：http://hz.fzhhl.top/gtdatrlmhx.html

[R55] 压缩与解压
来源：http://hz.jqgufenzy.top/gtmhernptf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.snrcjt.cn/gtevmidkdd.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gtzqfsmipv.html

scp file user@host:/path/
来源：http://hz.meibo888.top/gtagbwswbr.html

[R57] 远程执行命令
来源：http://hz.hysaishi.cn/gtautqqcaw.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtbxhuvagz.html

[R58] 下载文件
来源：http://hz.cheryme.top/gtigvpacvh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yanxiufei.cn/gtkqwdkpiw.html

[R59] 发 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtgwtevrap.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jqgfzy.top/gtpjwaedyn.html

[R60] 只看 HTTP 状态码
来源：http://hz.ybcxt.top/gtcpvdsjwy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shangyingyoupin.top/gtfivmtttu.html

[R61] 磁盘占用
来源：http://hz.cdnleiting.top/gtgdbyhetu.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtoaenjtws.html

[R62] 找最占空间的文件
来源：http://hz.hammf.cn/gtaarmqrrv.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxinkj.top/gtdlsxosiv.html

[R63] 内存与进程
来源：http://hz.cucudq.cn/gttaqcyzba.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258888.top/gtvqmslauq.html

[R64] 结束进程
来源：http://hz.meibo888.top/gtvncrlrfu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.0kj1m.cn/gtqbspdpfk.html

[R65] 查看端口占用
来源：http://hz.ydjk.org.cn/gthdzvwkts.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xylfe.cn/gtvikpmbgl.html

[R66] 定时任务
来源：http://hz.yueranfly.top/gtkfqmmdsa.html

crontab -e;  crontab -l
来源：http://hz.jyoumei.cn/gtzojrccby.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtnfzrlszu.html

openssl rand -hex 16
来源：http://hz.hnxiangtu.top/gtcnhoknii.html

[R68] 计算文件校验值
来源：http://hz.jiagoushi.top/gtyakmxtbf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhaomingkeji.xyz/gtkmgrizgw.html

[R69] 生成随机密码
来源：http://hz.xingfuxueyuan.xyz/gtrhvqkwln.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj202588.top/gtgksfntci.html

[R70] 时间戳与互转
来源：http://hz.vqdsnc.cn/gteqwbkzvs.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gtssidzjjr.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gttwuxuvho.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shangyingyoupin.top/gtizwrdcrj.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtqeohvtvz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtumcfojzm.html

[R73] 分割大日志
来源：http://hz.hnqzz.top/gtxmhzejww.html

split -l 1000 big.log part_
来源：http://hz.jqgufenzy.top/gtfloiwftb.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtvigfpsus.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ydjk.org.cn/gtzenjddjc.html

[R75] 导出环境变量
来源：http://hz.shuidangran.top/gtggqqfuvg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangdashe.top/gtmsiyprzg.html

[R76] 使用临时文件
来源：http://hz.jinqigfzy.top/gtjvndeiav.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtvxcdreji.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtmoirtfyk.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtrkqhawyb.html

[R78] 交互式菜单
来源：http://hz.svipenyu.cn/gtvsaibzgx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gotoacloud.top/gtudzkptnn.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gtfdokurdo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sysykeji.top/gtfntreqgd.html

[R80] 查看脚本执行耗时
来源：http://hz.zhixingplan.top/gtappxtmhj.html

time ./run.sh
来源：http://hz.chenzaomai.com/gtqhggrwkf.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgvakcuxs.html

S. C / C++ 专题
来源：http://hz.yanxiufei.cn/gtnemsdhae.html

================================================================================
来源：http://hz.yanxiufei.cn/gtudpppsys.html

[S01] C：Hello World
来源：http://hz.316326.xyz/gtubbcxpie.html

#include <stdio.h>
来源：http://hz.jinghuilouyu.cn/gtuatujcra.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shzxlz.cn/gtrjjwgjnd.html

[S02] C：变量与格式化输出
来源：http://hz.haohaochexian.top/gtoudoxwlo.html

int a = 10; printf("%d\n", a);
来源：http://hz.316326.xyz/gtaxsvfddo.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtduoszcaq.html

int x; scanf("%d", &x);
来源：http://hz.yuxming.cn/gttnsxcvuc.html

[S04] C：字符串复制
来源：http://hz.yanxiufei.cn/gtndbzspeb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jiagoushi.top/gtuluartyb.html

[S05] C：字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtyrzwfzij.html

strlen(s)
来源：http://hz.yuxming.cn/gtcdericyd.html

[S06] C：字符串比较
来源：http://hz.aibaodan.cn/gteqeoufjf.html

strcmp(a, b) == 0
来源：http://hz.zhixingplan.top/gthufonjve.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtrxazsjyr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gtudocdqjj.html

[S08] C：动态内存分配与释放
来源：http://hz.haohaochexian.top/gthteeqefl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gotoacloud.top/gtfvenwcnr.html

[S09] C：结构体定义与初始化
来源：http://hz.c1oappe.top/gtqvgyvzsf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jyoumei.cn/gtyrtjgtjx.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtgqmouaya.html

int *p = &a;  *p = 5;
来源：http://hz.xingfuxueyuan.xyz/gtnxwyhixb.html

[S11] C：逐行读文件
来源：http://hz.gogol.net.cn/gtocukvacn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtdjfoukbi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aizwys.cn/gtupikzhvv.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gtiwkppwya.html

[S12] C：写文件
来源：http://hz.shanyushiyangkeji.top/gtnkflosid.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ppjwa.cn/gtarsojeqq.html

[S13] C：宏定义
来源：http://hz.vqdsnc.cn/gtykwxqkez.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shuidangran.top/gtkwepqrqt.html

[S14] C：枚举
来源：http://hz.316326.xyz/gtsdtmgdet.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gttofikbrh.html

[S15] C：类型转换
来源：http://hz.zhixingplan.top/gtbaolyjyc.html

(double) a / b
来源：http://hz.9152youxi.cn/gtpymjzcvi.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtlngmjwgt.html

x |= (1 << 3);
来源：http://hz.sweek.top/gtyfqqqixv.html

[S17] C：安全拼接字符串
来源：http://hz.aizwys.cn/gtsehyjtoy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sxryk.cn/gtiqequuaa.html

[S18] C：命令行参数
来源：http://hz.tianlin.xyz/gtneiyybmx.html

int main(int argc, char **argv)
来源：http://hz.shangyingyoupin.top/gtvxavwczg.html

[S19] C：快速排序
来源：http://hz.dianchejie.cn/gtjihnuswo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtegvfuvzu.html

[S20] C：二分查找
来源：http://hz.chenlongwang.top/gtganvcqok.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.c1oappe.top/gtkbzpbhyz.html

[S21] C：字符类别判断
来源：http://hz.cdnleiting.top/gtdpdhofgx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj202588.top/gtvvsmmnyy.html

[S22] C：字符串转数字
来源：http://hz.yuxming.cn/gtihxsdkmy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.svipenyu.cn/gtjlotfdpm.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtlwvsjfxs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.meibo888.top/gttuiuvdnh.html

[S24] C：获取本地时间
来源：http://hz.cucudq.cn/gtlpshtnsz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tian-w.cn/gtbkmokstq.html

[S25] C：内存拷贝
来源：http://hz.dianchejie.cn/gtlphpoooj.html

memcpy(dst, src, n);
来源：http://hz.cucudq.cn/gtszvnbide.html

[S26] C：内存清零
来源：http://hz.cdnleiting.top/gtgbwcttrl.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gtphfydmzn.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtvixlvahl.html

const double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtmoapkmaj.html

[S28] C：静态变量
来源：http://hz.xziqi.cn/gtjgipgmhh.html

static int counter = 0;
来源：http://hz.wangdashe.top/gttycbqxme.html

[S29] C：变参函数
来源：http://hz.jinghuilouyu.cn/gtndgveyqu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnqzz.top/gtdckhxkts.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtjsykmqhz.html

#ifndef X_H
来源：http://hz.bjfxy.top/gtkdmriqen.html

#define X_H
来源：http://hz.aibaodan.cn/gtcgwlguas.html

#endif
来源：http://hz.daxiang520.top/gtplbyagnm.html

[S31] C++：Hello World
来源：http://hz.yuanzhike.top/gtwmacwece.html

#include <iostream>
来源：http://hz.xuanzx.com/gtzolvoban.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hfpthk.cn/gteswrswsi.html

[S32] C++：字符串
来源：http://hz.c1oappe.top/gtdydacrss.html

std::string s = "hi";  s += "!";
来源：http://hz.9152youxi.cn/gtfzolbrth.html

[S33] C++：vector 增删
来源：http://hz.zhijiandao.cn/gthrpnjcke.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dianchejie.cn/gteaptuzgl.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtjodacqrq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuxming.cn/gturiufmoc.html

[S35] C++：map
来源：http://hz.jqgfzy.top/gtczyihrpf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtouktilye.html

[S36] C++：unordered_map
来源：http://hz.jqgufenzy.top/gtklxcmasr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtgdrzhqqu.html

[S37] C++：set
来源：http://hz.tian-w.cn/gtiziojusj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sxryk.cn/gtrmicmwzy.html

[S38] C++：排序
来源：http://hz.zhongyouzk.top/gttwgcyptl.html

std::sort(v.begin(), v.end());
来源：http://hz.xziqi.cn/gtmwlozwxn.html

[S39] C++：自定义比较器排序
来源：http://hz.jlsjyb.cn/gtqrmnacka.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shangyingyoupin.top/gtyimcssvm.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtmbenbisg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinyuanbaomall.cn/gtaitrfwum.html

[S41] C++：类与构造函数
来源：http://hz.zhongyouzk.top/gtkwcqatmz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.wangshuangyany.cn/gtkufshdkz.html

[S42] C++：继承与虚函数
来源：http://hz.haohaochexian.top/gtiijotcke.html

class B : public Base { public: void f() override {} };
来源：http://hz.haohaochexian.top/gtzbelwwrw.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gtessuemgk.html

auto p = std::make_unique<int>(5);
来源：http://hz.ivvv.top/gttyuuymns.html

[S44] C++：引用传参
来源：http://hz.zdqjudy.top/gtqzccswsd.html

void inc(int &x) { ++x; }
来源：http://hz.wangdashe.top/gtyaaqwxgq.html

[S45] C++：lambda
来源：http://hz.svipenyu.cn/gtjrwybcaw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cqqwz.cn/gtptxmvapp.html

[S46] C++：函数模板
来源：http://hz.ppjwa.cn/gttvoljqii.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gthztijysi.html

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtksbguaar.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigufen.top/gttbtnqfxr.html

[S48] C++：逐行读文件
来源：http://hz.jqgufenzy.top/gtxbrmrnig.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgufenzy.top/gtdoinbkuy.html

while (std::getline(in, line)) { }
来源：http://hz.316326.xyz/gtvnfxgzfs.html

[S49] C++：写文件
来源：http://hz.nanxuanxn.top/gtymizleqk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fzhhl.top/gtgmuqmioa.html

[S50] C++：格式化数字
来源：http://hz.bjfxy.top/gtvsroqvtj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxuanxn.top/gtkcafwtae.html

[S51] C++：显式类型转换
来源：http://hz.nwbrower.top/gttgftlbrr.html

static_cast<double>(a) / b
来源：http://hz.jinqigufen.top/gttctvrumq.html

[S52] C++：const 与 noexcept
来源：http://hz.zhixingplan.top/gtygxmjobm.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtvfbobbvi.html

[S53] C++：移动语义
来源：http://hz.feifeiyinyue.top/gtstnragai.html

std::vector<int> w = std::move(v);
来源：http://hz.cashguo.top/gtmooxvjtq.html

[S54] C++：异常处理
来源：http://hz.gzhubu.top/gtoewmbmaw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenjidiqi.icu/gtxkrbzvrd.html

[S55] C++：结构化绑定
来源：http://hz.jlsjyb.cn/gtjedswobo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shzxlz.cn/gthhxhxyue.html

[S56] C++：optional
来源：http://hz.pycfn.com/gtfloenwjw.html


<!-- 参考信息 -->