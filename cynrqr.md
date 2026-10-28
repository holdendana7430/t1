代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.quarkkingdee.top/gtqnjfrfar.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.9152youxi.cn/gtinqnoqjz.html

[Q83] 大小写转换
来源：http://hz.cheryme.top/gtfrmstqez.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtgjnfszto.html

[Q84] 去除首尾空格
来源：http://hz.hongshengwenyu.top/gtnsluefbr.html

SELECT TRIM(name) FROM users;
来源：http://hz.yueranfly.top/gtynuingly.html

[Q85] 数值取整
来源：http://hz.ydzc1.top/gtoltcvert.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhixingplan.top/gtoamutpyc.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtlrzsoazg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xziqi.cn/gtqdstibjv.html

[Q87] JSON 字段做条件
来源：http://hz.c1oappe.top/gtlltlhrlk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtfmmjyhvi.html

[Q88] 行转列（条件聚合）
来源：http://hz.tanke756.top/gtxncctxjw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnxiangtu.top/gtfnpxlgdx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shuidangran.top/gtfalbymhz.html

[Q89] 判断表是否存在
来源：http://hz.sweek.top/gtuljqlifj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtagufgfvo.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtbgelsgdb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.0kj1m.cn/gtdctqhltd.html

================================================================================
来源：http://hz.316326.xyz/gtaebfqcjk.html

R. Bash 专题
来源：http://hz.zhiwuduotai.top/gtuolcibeo.html

================================================================================
来源：http://hz.birdmap.top/gtqsalbecb.html

[R01] shebang 与严格模式
来源：http://hz.52xcode.cn/gtzsstofsb.html

#!/usr/bin/env bash
来源：http://hz.andypj.xyz/gtinhoquis.html

set -euo pipefail
来源：http://hz.vqdsnc.cn/gtihqaxjgi.html

[R02] 变量赋值与使用
来源：http://hz.zhaomingkeji.xyz/gtkqevkwmg.html

name="Tom"; echo "$name"
来源：http://hz.jinyuanbaomall.cn/gtvzhwfjyx.html

[R03] 只读变量
来源：http://hz.zdqjudy.top/gtshvsyprk.html

readonly PI=3.14
来源：http://hz.daxiang520.top/gthrhjmijg.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gtctnsvxjf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.birdmap.top/gteafzjdty.html

[R05] 参数默认值
来源：http://hz.hongshengwenyu.top/gtggwyvpaf.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtayxiazoy.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtpnczvcci.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gtusmmdsvd.html

[R07] if 判断文件
来源：http://hz.aibaodan.cn/gtjcfptfed.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhijiandao.cn/gtudjtuqoe.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gtectweiil.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sufxvd.cn/gtmwjbnsgq.html

[R09] 字符串比较
来源：http://hz.yvedp.cn/gtoyndnbnz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hammf.cn/gtkglkntyr.html

[R10] 正则匹配
来源：http://hz.sxryk.cn/gtbigmhlcu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gtgjnmrxlp.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtbcfbnvtp.html

case "$1" in
来源：http://hz.yuxming.cn/gtuvbgwgrb.html

start) echo "启动" ;;
来源：http://hz.meibo888.top/gtanpagikw.html

stop)  echo "停止" ;;
来源：http://hz.yongpay.top/gtdubjnnjz.html

*)     echo "未知命令" ;;
来源：http://hz.nanxuanxn.top/gtiwnlakfm.html

esac
来源：http://hz.tanke756.top/gtngceisrl.html

[R12] for 遍历文件
来源：http://hz.yj20258.top/gtkcovhobt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sweek.top/gtitxxbbew.html

[R13] for 计数循环
来源：http://hz.zhijiandao.cn/gtffoadrsu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gtzlzraubn.html

[R14] C 风格 for
来源：http://hz.xziqi.cn/gtbtlloqiq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtxowuidgd.html

[R15] while 逐行读文件
来源：http://hz.ivvv.top/gtxxvdukxk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zycfv.cn/gtvsxqityf.html

[R16] until 等待条件
来源：http://hz.mhx1999.top/gtttgembbj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtxpuhicjz.html

[R17] 数组定义与取值
来源：http://hz.yuanzhike.top/gtngppvlvq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuetiantiany.cn/gtdsukeljp.html

[R18] 遍历数组
来源：http://hz.jqgfzy.top/gtgojwzqya.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.kuanghao11.cn/gtfzgiuviu.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtmgdicswh.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtryavtwad.html

[R20] 关联数组（字典）
来源：http://hz.cheryme.top/gtyydvswgv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nwbrower.top/gtctthzazo.html

[R21] 字符串长度
来源：http://hz.gaohongyu789.top/gtajpfimra.html

echo "${#s}"
来源：http://hz.zycfv.cn/gtaeullapv.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtpuprrmag.html

echo "${s:0:5}"
来源：http://hz.meibo888.top/gttxqzeess.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtbjjkxzzs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gtsdoyzkro.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtvgtofwvi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtzxxgaycu.html

[R25] 去后缀 / 去前缀
来源：http://hz.ppjwa.cn/gtnduolzgl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtdyuytgsk.html

[R26] 命令替换
来源：http://hz.zhoulong.xyz/gtmpdrclvs.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gtpowsgyiw.html

[R27] 算术展开
来源：http://hz.zhixingplan.top/gtokudmarr.html

echo $((1 + 2 * 3))
来源：http://hz.yonumen.top/gtxmiuxvns.html

[R28] 浮点运算
来源：http://hz.haohaochexian.top/gtmzdgtqav.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnqzz.top/gtjztqqkfc.html

[R29] 定义函数
来源：http://hz.chenjidiqi.icu/gteogtizzc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gtohqosftf.html

[R30] 函数返回状态码
来源：http://hz.cashguo.top/gtzdahfafu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nwbrower.top/gtzoixkchl.html

[R31] 局部变量
来源：http://hz.sxryk.cn/gtanglgltj.html

f() { local x=1; echo "$x"; }
来源：http://hz.tanke756.top/gtnlyhwcwy.html

[R32] 参数个数校验
来源：http://hz.sufxvd.cn/gtnwyvlyua.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jyoumei.cn/gtcncpdiid.html

[R33] 捕获错误并提示行号
来源：http://hz.zhongyouzk.top/gttkssroes.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangtech.top/gtkzjalvmw.html

[R34] 退出时清理
来源：http://hz.feifeiyinyue.top/gtdsxmwvhs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtgginxefk.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangkeji.top/gtfywfkoog.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtbwmfethh.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtdxaffboh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgufenzy.top/gtwuftuijo.html

[R37] 把输出赋给变量
来源：http://hz.guannengcc.top/gthyocngjh.html

files=$(ls -1)
来源：http://hz.zycfv.cn/gtacxwjsao.html

[R38] 管道串联
来源：http://hz.wangshuangyany.cn/gthepkgbva.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtbzodoeir.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258888.top/gtfpmidetg.html

cmd > out.log 2>&1
来源：http://hz.yj20258.top/gtuxnuqeyb.html

[R40] 追加写日志
来源：http://hz.meibo888.top/gtwkayjxcp.html

echo "log" >> out.log
来源：http://hz.c1oappe.top/gtugptvvie.html

[R41] 丢弃输出
来源：http://hz.tanke756.top/gtemixoheu.html

cmd >/dev/null 2>&1
来源：http://hz.iojbl.cn/gtywkpcozu.html

[R42] 输入重定向
来源：http://hz.jinqigfzy.top/gtdzsrsvim.html

wc -l < a.txt
来源：http://hz.gaohongyu789.top/gtvipdzjyn.html

[R43] 按名字查找文件
来源：http://hz.fzhhl.top/gtmgqddwqe.html

find . -name "*.log" -type f
来源：http://hz.shzxlz.cn/gtogyruqbq.html

[R44] 按修改时间查找
来源：http://hz.jinqigfzy.top/gtwltegijt.html

find . -mtime -7 -type f
来源：http://hz.yj20258888.top/gtywphubwz.html

[R45] 批量删除
来源：http://hz.ehwqpu.com/gtfqhyyvuw.html

find . -name "*.tmp" -delete
来源：http://hz.yuanzhike.top/gtqtvvscrb.html

[R46] 递归替换文件内容
来源：http://hz.aibaodan.cn/gtqvadfxel.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.redwolf501.top/gthjpwsmza.html

[R47] sed 单行替换
来源：http://hz.mhx1999.top/gtumacpsfs.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sufxvd.cn/gtvyjrrjvn.html

[R48] awk 取指定列
来源：http://hz.sysykeji.top/gtzurmotby.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gtaynyrsel.html

[R49] awk 带条件
来源：http://hz.hongshengwenyu.top/gttvqjlwnn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tianlin.xyz/gtceivhwyt.html

[R50] awk 求和
来源：http://hz.smart0.xyz/gtafbwmlvr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sufxvd.cn/gtguilyhui.html

[R51] 排序去重取前几
来源：http://hz.chenlongwang.top/gtypcdliku.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhoulong.xyz/gthzgjmozu.html

[R52] 统计行数
来源：http://hz.pycfn.com/gtvfmkfxci.html

wc -l a.txt
来源：http://hz.shanyushiyangtech.top/gtxcnpyimy.html

[R53] 查看文件头与实时尾
来源：http://hz.yvedp.cn/gtztazoxdm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yanxiufei.cn/gtcaggpyxw.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gtywwseizh.html

diff a.txt b.txt
来源：http://hz.jqgufenzy.top/gtydvbbfnw.html

[R55] 压缩与解压
来源：http://hz.cashguo.top/gtoreoehyt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hywenlv.cn/gtyuhiawkr.html

[R56] 远程拷贝
来源：http://hz.yj20258888.top/gtdcfjxcuv.html

scp file user@host:/path/
来源：http://hz.wangshuangyany.cn/gtrxlkzsli.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtqzlrlvvm.html

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtpyzarjjc.html

[R58] 下载文件
来源：http://hz.hnqzz.top/gtcatveykj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gtjtbzustj.html

[R59] 发 POST JSON
来源：http://hz.andypj.xyz/gtpxhxtord.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangkeji.top/gtvetplbox.html

[R60] 只看 HTTP 状态码
来源：http://hz.ydjk.org.cn/gtfyxvlfyh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cqqwz.cn/gtphdpryvi.html

[R61] 磁盘占用
来源：http://hz.nanxinkj.top/gtmenxaogx.html

df -h;  du -sh *
来源：http://hz.tanke756.top/gtgfkyywsy.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gtirglhdcv.html

du -ah . | sort -rh | head -10
来源：http://hz.gzhubu.top/gtrkicjorn.html

[R63] 内存与进程
来源：http://hz.ywan-chungtsiang.top/gtwszvnqgl.html

free -h;  ps aux | grep nginx
来源：http://hz.yj202588.top/gtwfcvkcad.html

[R64] 结束进程
来源：http://hz.jinqigfzy.top/gttwhsgykw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cashguo.top/gtugcsdddx.html

[R65] 查看端口占用
来源：http://hz.shuidangran.top/gtsrzcpkvl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jlsjyb.cn/gththquwwr.html

[R66] 定时任务
来源：http://hz.fzhhl.top/gtyhtsutje.html

crontab -e;  crontab -l
来源：http://hz.chenlongwang.top/gtnihyvxvu.html

[R67] 生成随机十六进制串
来源：http://hz.yvedp.cn/gtxfhntzpm.html

openssl rand -hex 16
来源：http://hz.ppjwa.cn/gthokgeabk.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gtipygiofr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.c1oappe.top/gtnrpnsbib.html

[R69] 生成随机密码
来源：http://hz.zdqjudy.top/gtwhwudwia.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhijiandao.cn/gtfafqcohf.html

[R70] 时间戳与互转
来源：http://hz.fzhhl.top/gtdcyuvmia.html

date +%s;  date -d @1700000000
来源：http://hz.gotoacloud.top/gtksmezdcx.html

[R71] 日期格式化
来源：http://hz.jiagoushi.top/gtlflyyvxh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daria6918.cn/gtnjgsifoe.html

[R72] 等待端口就绪
来源：http://hz.chenlongwang.top/gthoyeoxbi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj202588.top/gtiiczyeca.html

[R73] 分割大日志
来源：http://hz.aizwys.cn/gtqwjyufih.html

split -l 1000 big.log part_
来源：http://hz.zhengqikj.top/gtictyqkmc.html

[R74] 批量重命名
来源：http://hz.aizwys.cn/gtpoodygzq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gogol.net.cn/gtwckmzauo.html

[R75] 导出环境变量
来源：http://hz.zhiwuduotai.top/gthdjgqyah.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nwbrower.top/gtqjjctgxd.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gthkqizick.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtffsnzhkj.html

[R77] 读取用户输入
来源：http://hz.hywenlv.cn/gtjcnvytgs.html

read -rp "请输入: " ans
来源：http://hz.cdnleiting.top/gtlbgopqtc.html

[R78] 交互式菜单
来源：http://hz.shuidangran.top/gtklfuznah.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yvedp.cn/gtqbyxwrqo.html

[R79] 解析命令行选项
来源：http://hz.nwbrower.top/gtybzqtkcj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtvlosqmcx.html

[R80] 查看脚本执行耗时
来源：http://hz.cqqwz.cn/gtgupcjqbt.html

time ./run.sh
来源：http://hz.ywan-chungtsiang.top/gtaxzoxpva.html

================================================================================
来源：http://hz.sysykeji.top/gtasjvnqbw.html

S. C / C++ 专题
来源：http://hz.xinyue.icu/gtxoqgtgtk.html

================================================================================
来源：http://hz.gzhubu.top/gtkhwibeut.html

[S01] C：Hello World
来源：http://hz.svipenyu.cn/gtutauyopl.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtlagtqrld.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shanyushiyangtech.top/gtavnohluf.html

[S02] C：变量与格式化输出
来源：http://hz.zycfv.cn/gtntdpdsky.html

int a = 10; printf("%d\n", a);
来源：http://hz.hfpthk.cn/gtajrihwyk.html

[S03] C：读入整数
来源：http://hz.xylfe.cn/gtmclfkwkf.html

int x; scanf("%d", &x);
来源：http://hz.yj20258888.top/gtvkietyhi.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtrnhnuehu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.dashuyun.cn/gtizjrdpxp.html

[S05] C：字符串长度
来源：http://hz.0kj1m.cn/gtgtulqztj.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtruyfeuen.html

[S06] C：字符串比较
来源：http://hz.havefunace.top/gtieowzwae.html

strcmp(a, b) == 0
来源：http://hz.jqgfzy.top/gtbpvaerds.html

[S07] C：数组遍历求和
来源：http://hz.tanke756.top/gtvngrhoaw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gtxmnetkbj.html

[S08] C：动态内存分配与释放
来源：http://hz.jiagoushi.top/gtpceqgubk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.c1oappe.top/gtzvxdsgyr.html

[S09] C：结构体定义与初始化
来源：http://hz.aizwys.cn/gtlxjurjnw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guannengcc.top/gtystwtghc.html

[S10] C：指针与解引用
来源：http://hz.9152youxi.cn/gtahahlwgz.html

int *p = &a;  *p = 5;
来源：http://hz.jlsjyb.cn/gtaqwsilan.html

[S11] C：逐行读文件
来源：http://hz.kuanghao11.cn/gtedikjpab.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtezyqmqbj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xylfe.cn/gtspfmmtpv.html

fclose(f);
来源：http://hz.zdqjudy.top/gtxfehohdl.html

[S12] C：写文件
来源：http://hz.cqqwz.cn/gtrjouhkqj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258.top/gtrssvostq.html

[S13] C：宏定义
来源：http://hz.jinyuanbaomall.cn/gtzkcqmwkv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxinkj.top/gtmwzwpzwj.html

[S14] C：枚举
来源：http://hz.316326.xyz/gtygykibrm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.mhx1999.top/gtkxnwfyeb.html

[S15] C：类型转换
来源：http://hz.xinyue.icu/gtahumeayc.html

(double) a / b
来源：http://hz.hongshengwenyu.top/gtmwcianhs.html

[S16] C：位操作置位
来源：http://hz.yj20258.top/gtzcqodsar.html

x |= (1 << 3);
来源：http://hz.ydzc1.top/gtijvvbjan.html

[S17] C：安全拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtqvcleify.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ywan-chungtsiang.top/gttxliadxe.html

[S18] C：命令行参数
来源：http://hz.xylfe.cn/gtnllwdfyt.html

int main(int argc, char **argv)
来源：http://hz.nwbrower.top/gtuvagqlrg.html

[S19] C：快速排序
来源：http://hz.tianlin.xyz/gtkhjaxdtv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtmufwpwyz.html

[S20] C：二分查找
来源：http://hz.xingfuxueyuan.xyz/gtcugeuhnm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtcwagcddn.html

[S21] C：字符类别判断
来源：http://hz.jyoumei.cn/gtmnqjqskl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hongshengwenyu.top/gtbkzistns.html

[S22] C：字符串转数字
来源：http://hz.smart0.xyz/gtbtujmuez.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhixingplan.top/gtskqrrnqx.html

[S23] C：随机数
来源：http://hz.52xcode.cn/gtldakzdcn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ywan-chungtsiang.top/gttocjngtp.html

[S24] C：获取本地时间
来源：http://hz.cqqwz.cn/gtiwejbkkx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhoulong.xyz/gtwukpvgkv.html

[S25] C：内存拷贝
来源：http://hz.yonumen.top/gtmvsujykd.html

memcpy(dst, src, n);
来源：http://hz.jiagoushi.top/gtulfpdlfa.html

[S26] C：内存清零
来源：http://hz.sysykeji.top/gtnknhhhao.html

memset(a, 0, sizeof a);
来源：http://hz.316326.xyz/gtikwlcepe.html

[S27] C：定义常量
来源：http://hz.nanxuanxn.top/gtsfmqebdg.html

const double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtdorauzba.html

[S28] C：静态变量
来源：http://hz.fengsongda.top/gtqbgqdjsm.html

static int counter = 0;
来源：http://hz.jyoumei.cn/gtglvfgznu.html

[S29] C：变参函数
来源：http://hz.dashuyun.cn/gtwhafxgcn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.svipenyu.cn/gtahmhdtjb.html

[S30] C：头文件保护
来源：http://hz.yonumen.top/gtklfafitl.html

#ifndef X_H
来源：http://hz.quarkkingdee.top/gtneclywis.html

#define X_H
来源：http://hz.shzxlz.cn/gtphiqrhxp.html

#endif
来源：http://hz.zdqjudy.top/gtyyrhkrqn.html

[S31] C++：Hello World
来源：http://hz.fengsongda.top/gthzrulsyv.html

#include <iostream>
来源：http://hz.havefunace.top/gtxvyimlyv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gtjzsbckoa.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtvhnledmz.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtvkweshtw.html

[S33] C++：vector 增删
来源：http://hz.zycfv.cn/gtsclxrwft.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhijiandao.cn/gtgltlhguu.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gthhrojudu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxinkj.top/gtxdbuigjr.html

[S35] C++：map
来源：http://hz.mhx1999.top/gtsplgrnct.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtasmljezi.html

[S36] C++：unordered_map
来源：http://hz.aibaodan.cn/gtgxeqlwem.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hongshengwenyu.top/gtiqankcde.html

[S37] C++：set
来源：http://hz.shuidangran.top/gtdjgkrlok.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cqqwz.cn/gtdgyuszji.html

[S38] C++：排序
来源：http://hz.cucudq.cn/gtunfcvjnn.html

std::sort(v.begin(), v.end());
来源：http://hz.wangdashe.top/gthqozyehi.html

[S39] C++：自定义比较器排序
来源：http://hz.wangdashe.top/gtbqihaxiw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fzhhl.top/gtzodaeqkq.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtwwhlvrxc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.birdmap.top/gtnsjpsgfp.html

[S41] C++：类与构造函数
来源：http://hz.meibo888.top/gtfptpwmfg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtpjmrpluo.html

[S42] C++：继承与虚函数
来源：http://hz.guowangkeji.top/gtndsnuqud.html

class B : public Base { public: void f() override {} };
来源：http://hz.gaohongyu789.top/gtzgmquecg.html

[S43] C++：智能指针
来源：http://hz.ybcxt.top/gtbvueadif.html

auto p = std::make_unique<int>(5);
来源：http://hz.cheryme.top/gtndxbmtrx.html

[S44] C++：引用传参
来源：http://hz.zhaomingkeji.xyz/gtztowxign.html

void inc(int &x) { ++x; }
来源：http://hz.jianghu66.top/gtaangxvgv.html

[S45] C++：lambda
来源：http://hz.svipenyu.cn/gtnqvjdtqe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.havefunace.top/gtnfyhhvps.html

[S46] C++：函数模板
来源：http://hz.xziqi.cn/gtstketdwe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.smart0.xyz/gtzkpfhyss.html

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtrnykfuhg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gotoacloud.top/gtxjvxdtls.html

[S48] C++：逐行读文件
来源：http://hz.andypj.xyz/gtqyupufxq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.quarkkingdee.top/gtijqjmfve.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangtech.top/gthkwrkvgz.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtfekwydks.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.52xcode.cn/gtwubmjyxt.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gtdeaevgxg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj202588.top/gtemmhpbou.html

[S51] C++：显式类型转换
来源：http://hz.xinyue.icu/gterezfhmb.html

static_cast<double>(a) / b
来源：http://hz.52xcode.cn/gtkqhpuexo.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gthldypfbh.html


<!-- 参考信息 -->