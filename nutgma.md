代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.sufxvd.cn/gtekpasspw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtmedmljmp.html

[Q87] JSON 字段做条件
来源：http://hz.yvedp.cn/gtdwsojgpi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.c1oappe.top/gtxqzulfvj.html

[Q88] 行转列（条件聚合）
来源：http://hz.andypj.xyz/gtyzuzgnoi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gtejvojnnq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.meibo888.top/gthyxgkguv.html

[Q89] 判断表是否存在
来源：http://hz.yueranfly.top/gtqmtzwihc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gtiudxrzyt.html

[Q90] 生成序号列
来源：http://hz.hysaishi.cn/gtmdcbzxas.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gaohongyu789.top/gtlurhjlnd.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlhkcofcs.html

R. Bash 专题
来源：http://hz.cdnleiting.top/gtwaadvefb.html

================================================================================
来源：http://hz.jyoumei.cn/gtuxzqgdba.html

[R01] shebang 与严格模式
来源：http://hz.yvedp.cn/gtqljuwiel.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gtiedquszv.html

set -euo pipefail
来源：http://hz.yuxming.cn/gtafcxdnpq.html

[R02] 变量赋值与使用
来源：http://hz.zhixingplan.top/gthkmlgelw.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gtypyqqeye.html

[R03] 只读变量
来源：http://hz.xylfe.cn/gtiwogfhyg.html

readonly PI=3.14
来源：http://hz.redwolf501.top/gtwryscegd.html

[R04] 位置参数
来源：http://hz.aibaodan.cn/gtznasudoq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gzhubu.top/gtdpsittsz.html

[R05] 参数默认值
来源：http://hz.yj20258888.top/gtwazgpmzt.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gtxsxcypbq.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtsfrgrgth.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gttxbaotss.html

[R07] if 判断文件
来源：http://hz.yongpay.top/gtejtfbmfa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ppjwa.cn/gtbcgzfsgs.html

[R08] 数值比较
来源：http://hz.pengpengdd.cyou/gtmzgccyqr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yueranfly.top/gtpcnvhlic.html

[R09] 字符串比较
来源：http://hz.zhongyouzk.top/gtqlnxlwgu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jiagoushi.top/gttnysdjwp.html

[R10] 正则匹配
来源：http://hz.hongshengwenyu.top/gtlollrnfs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dashuyun.cn/gtxgkebadj.html

[R11] case 多分支
来源：http://hz.sufxvd.cn/gtifhfmrha.html

case "$1" in
来源：http://hz.hysaishi.cn/gttbzvhepd.html

start) echo "启动" ;;
来源：http://hz.zycfv.cn/gtdxiojupe.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtsycareai.html

*)     echo "未知命令" ;;
来源：http://hz.haohaochexian.top/gtkzrueuyd.html

esac
来源：http://hz.dianchejie.cn/gtxipvbnpc.html

[R12] for 遍历文件
来源：http://hz.chenjidiqi.icu/gtkanylbwg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tanke756.top/gtlkgdlysr.html

[R13] for 计数循环
来源：http://hz.shanyushiyangtech.top/gtdkyermjf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dashuyun.cn/gtvvlrijap.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtzlfsuoch.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.meibo888.top/gtxlamorzw.html

[R15] while 逐行读文件
来源：http://hz.316326.xyz/gtazpdehfc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dashuyun.cn/gtbkpzcmqt.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gthvzmercs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gtborfoosc.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtaziaywzx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinyuanbaomall.cn/gttwsttcvz.html

[R18] 遍历数组
来源：http://hz.gzhubu.top/gtrkjzcfvt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gthvzhlamf.html

[R19] 数组长度
来源：http://hz.guowangkeji.top/gtgzrbxblv.html

echo "${#arr[@]}"
来源：http://hz.gotoacloud.top/gtnawfcsbe.html

[R20] 关联数组（字典）
来源：http://hz.gogol.net.cn/gtznheistk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yanxiufei.cn/gtcsaxmhtb.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtfzzrpnyr.html

echo "${#s}"
来源：http://hz.cucudq.cn/gtbmerieif.html

[R22] 截取子串
来源：http://hz.0kj1m.cn/gtyizvnerd.html

echo "${s:0:5}"
来源：http://hz.c1oappe.top/gtpgloxxzv.html

[R23] 字符串替换
来源：http://hz.meibo888.top/gtkmphbrdn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigufen.top/gtjpcdvzbo.html

[R24] 大小写转换
来源：http://hz.cdnleiting.top/gtsskcgdhc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtmoiasuad.html

[R25] 去后缀 / 去前缀
来源：http://hz.xingfuxueyuan.xyz/gtecoprwkj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtsktxvhiu.html

[R26] 命令替换
来源：http://hz.sxryk.cn/gttqouhkie.html

now=$(date +%F); echo "$now"
来源：http://hz.yvedp.cn/gtxogutnnp.html

[R27] 算术展开
来源：http://hz.fzhhl.top/gtdbsmmmus.html

echo $((1 + 2 * 3))
来源：http://hz.yueranfly.top/gtpnpaicmy.html

[R28] 浮点运算
来源：http://hz.yangfankeji.com/gtuvzrwaxk.html

echo "scale=2; 10/3" | bc
来源：http://hz.zdqjudy.top/gtbmhtxjfe.html

[R29] 定义函数
来源：http://hz.yonumen.top/gtulrrzqnd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.snrcjt.cn/gtregaisjq.html

[R30] 函数返回状态码
来源：http://hz.xziqi.cn/gtiubxpxzv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nwbrower.top/gthtfswyed.html

[R31] 局部变量
来源：http://hz.sysykeji.top/gtajpdrmpc.html

f() { local x=1; echo "$x"; }
来源：http://hz.cashguo.top/gtkrmaeyxu.html

[R32] 参数个数校验
来源：http://hz.guannengcc.top/gtbcpczrvy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.havefunace.top/gtjebrtxok.html

[R33] 捕获错误并提示行号
来源：http://hz.wangdashe.top/gtdukptkkw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ehwqpu.com/gtscxgfjws.html

[R34] 退出时清理
来源：http://hz.feifeiyinyue.top/gtlcpthjfx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtrwpuitgf.html

[R35] 后台执行并等待
来源：http://hz.zycfv.cn/gtfbwqktkh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sufxvd.cn/gtxvbugxrn.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtherukteu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.9152youxi.cn/gtyrpoedoc.html

[R37] 把输出赋给变量
来源：http://hz.jianghu66.top/gthdhfafza.html

files=$(ls -1)
来源：http://hz.yueranfly.top/gtiriobjvg.html

[R38] 管道串联
来源：http://hz.ehwqpu.com/gtqzmqbsmb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenzaomai.com/gtcwrqfpza.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gtlqkhcdhg.html

cmd > out.log 2>&1
来源：http://hz.nanxuanxn.top/gtsibsgwbe.html

[R40] 追加写日志
来源：http://hz.vqdsnc.cn/gtewivtbpq.html

echo "log" >> out.log
来源：http://hz.yangfankeji.com/gtcpyfrrna.html

[R41] 丢弃输出
来源：http://hz.chenlongwang.top/gtufrrxtgv.html

cmd >/dev/null 2>&1
来源：http://hz.chenjidiqi.icu/gtvyauiakj.html

[R42] 输入重定向
来源：http://hz.jqgufenzy.top/gtwxjfyfez.html

wc -l < a.txt
来源：http://hz.zhixingplan.top/gttczzohzp.html

[R43] 按名字查找文件
来源：http://hz.xinyue.icu/gtliskycbx.html

find . -name "*.log" -type f
来源：http://hz.yj20258.top/gtjjejpusu.html

[R44] 按修改时间查找
来源：http://hz.jqgufenzy.top/gttxfrkkpf.html

find . -mtime -7 -type f
来源：http://hz.hammf.cn/gtlisuoypr.html

[R45] 批量删除
来源：http://hz.yj202588.top/gtbmdpkycs.html

find . -name "*.tmp" -delete
来源：http://hz.haohaochexian.top/gtjplbozwb.html

[R46] 递归替换文件内容
来源：http://hz.zhijiandao.cn/gtimkftjlj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xinyue.icu/gtpasxmzyh.html

[R47] sed 单行替换
来源：http://hz.guowangkeji.top/gtlxmnfgry.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxinkj.top/gttccesgta.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gtyrgpfgbh.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gtpxveknnp.html

[R49] awk 带条件
来源：http://hz.chenjidiqi.icu/gtzidljqty.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gtwoqjqktd.html

[R50] awk 求和
来源：http://hz.jinghuilouyu.cn/gtzujlmekc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zdqjudy.top/gtmqvzkozi.html

[R51] 排序去重取前几
来源：http://hz.dashuyun.cn/gtjfcdekaa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cqqwz.cn/gtzvpgxzdg.html

[R52] 统计行数
来源：http://hz.52xcode.cn/gtxhwdcpfb.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gtbbmgxswn.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtkfajnhek.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gtbdbbqbav.html

[R54] 比较两个文件
来源：http://hz.c1oappe.top/gtvfwgcisf.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtdszgrkve.html

[R55] 压缩与解压
来源：http://hz.yvedp.cn/gtfryvkhzj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtcsixwflp.html

[R56] 远程拷贝
来源：http://hz.gaohongyu789.top/gtifmfseny.html

scp file user@host:/path/
来源：http://hz.iojbl.cn/gtjmcatyod.html

[R57] 远程执行命令
来源：http://hz.jqgfzy.top/gtjabrgamg.html

ssh user@host 'uptime'
来源：http://hz.daria6918.cn/gtubbkoemn.html

[R58] 下载文件
来源：http://hz.jyoumei.cn/gtfqzakxzo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtexmdcrjx.html

[R59] 发 POST JSON
来源：http://hz.hnqzz.top/gtbnogobuv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gaohongyu789.top/gtcaxjuyli.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtawmuotvz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xingfuxueyuan.xyz/gttfuhgbts.html

[R61] 磁盘占用
来源：http://hz.zycfv.cn/gtgcvdujdj.html

df -h;  du -sh *
来源：http://hz.birdmap.top/gtpnbmxeqw.html

[R62] 找最占空间的文件
来源：http://hz.52xcode.cn/gtgjhknenm.html

du -ah . | sort -rh | head -10
来源：http://hz.cashguo.top/gtbuynrboi.html

[R63] 内存与进程
来源：http://hz.cqqwz.cn/gtwwfkdyvi.html

free -h;  ps aux | grep nginx
来源：http://hz.wangdashe.top/gtpytwnzae.html

[R64] 结束进程
来源：http://hz.zhixingplan.top/gtcxfuwxge.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sweek.top/gthbrluzir.html

[R65] 查看端口占用
来源：http://hz.meibo888.top/gtgdavcrpw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shzxlz.cn/gtebycgphk.html

[R66] 定时任务
来源：http://hz.yonumen.top/gtmkuhcpso.html

crontab -e;  crontab -l
来源：http://hz.jiagoushi.top/gtxqevlzgl.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigufen.top/gttmxceptx.html

openssl rand -hex 16
来源：http://hz.zycfv.cn/gtauxfushl.html

[R68] 计算文件校验值
来源：http://hz.52xcode.cn/gtpxcbnlvp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxuanxn.top/gtywgemswi.html

[R69] 生成随机密码
来源：http://hz.yj202588.top/gtvnmwsaya.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258.top/gtbqgflkyw.html

[R70] 时间戳与互转
来源：http://hz.guannengcc.top/gtbnpgrbsd.html

date +%s;  date -d @1700000000
来源：http://hz.shzxlz.cn/gtjigolxtw.html

[R71] 日期格式化
来源：http://hz.gzhubu.top/gtnzmspvja.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtuaapgqrx.html

[R72] 等待端口就绪
来源：http://hz.shangyingyoupin.top/gtsfskhyec.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dianchejie.cn/gtqhokdrud.html

[R73] 分割大日志
来源：http://hz.nanxinkj.top/gteizuoifa.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtmvobfoyl.html

[R74] 批量重命名
来源：http://hz.quarkkingdee.top/gtgrrtesmv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigfzy.top/gtuomwjetr.html

[R75] 导出环境变量
来源：http://hz.chenzaomai.com/gtkzewcduj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tanke756.top/gtrqhdezod.html

[R76] 使用临时文件
来源：http://hz.nanxuanxn.top/gtujmzxkiw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gtcyevygnt.html

[R77] 读取用户输入
来源：http://hz.zhoulong.xyz/gtihtpltmm.html

read -rp "请输入: " ans
来源：http://hz.zhixingplan.top/gtvufftzmd.html

[R78] 交互式菜单
来源：http://hz.vqdsnc.cn/gtirzmvxmq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhiwuduotai.top/gtapybvpma.html

[R79] 解析命令行选项
来源：http://hz.hnqzz.top/gtivudusco.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.mhx1999.top/gtlskapaff.html

[R80] 查看脚本执行耗时
来源：http://hz.nwbrower.top/gtmmpbdvhg.html

time ./run.sh
来源：http://hz.gaohongyu789.top/gtmpaohgeu.html

================================================================================
来源：http://hz.yangfankeji.com/gtwjjvnfjw.html

S. C / C++ 专题
来源：http://hz.gotoacloud.top/gtlingzebn.html

================================================================================
来源：http://hz.sxryk.cn/gtyqafewwj.html

[S01] C：Hello World
来源：http://hz.sysykeji.top/gtuxcaxryv.html

#include <stdio.h>
来源：http://hz.yuanzhike.top/gtqgdsupud.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.52xcode.cn/gtxcnridzs.html

[S02] C：变量与格式化输出
来源：http://hz.xziqi.cn/gtczwududn.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhengqikj.top/gtwjnaokfn.html

[S03] C：读入整数
来源：http://hz.gzhubu.top/gtjljdlpfa.html

int x; scanf("%d", &x);
来源：http://hz.jqgufenzy.top/gtwwiryeqm.html

[S04] C：字符串复制
来源：http://hz.sweek.top/gtzaehcbks.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guannengcc.top/gtasxncdpe.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtcwuafvly.html

strlen(s)
来源：http://hz.gotoacloud.top/gtikjobgpo.html

[S06] C：字符串比较
来源：http://hz.ivvv.top/gtmwvjuqsx.html

strcmp(a, b) == 0
来源：http://hz.zhaomingkeji.xyz/gtswldxobn.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gtioilukit.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ehwqpu.com/gtgvtdcsky.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtsvbulmmj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtilpdndrw.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxuanxn.top/gtqoepmcml.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cashguo.top/gtpqvdlvge.html

[S10] C：指针与解引用
来源：http://hz.yj202588.top/gtmhmcpfkl.html

int *p = &a;  *p = 5;
来源：http://hz.quarkkingdee.top/gtsmvmdmpb.html

[S11] C：逐行读文件
来源：http://hz.vqdsnc.cn/gtkobecscf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtxeynvcox.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.bjfxy.top/gtvmngqsom.html

fclose(f);
来源：http://hz.chenjidiqi.icu/gtqcpmbwtw.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtichilvvi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj202588.top/gtketimtol.html

[S13] C：宏定义
来源：http://hz.zhaomingkeji.xyz/gtdjlxmmqq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.c1oappe.top/gtudskyzbk.html

[S14] C：枚举
来源：http://hz.yangfankeji.com/gttissxgyg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gtivxtmdga.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gtluhlpdlo.html

(double) a / b
来源：http://hz.xuetiantiany.cn/gtlgnjmxnf.html

[S16] C：位操作置位
来源：http://hz.shzxlz.cn/gttsscfsgi.html

x |= (1 << 3);
来源：http://hz.gaohongyu789.top/gtqsviodiq.html

[S17] C：安全拼接字符串
来源：http://hz.zhixingplan.top/gtanxrquqw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenjidiqi.icu/gtuovqfjpn.html

[S18] C：命令行参数
来源：http://hz.jyoumei.cn/gtznycfwuc.html

int main(int argc, char **argv)
来源：http://hz.hnqzz.top/gtzqbznhad.html

[S19] C：快速排序
来源：http://hz.sysykeji.top/gtseocelja.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtfsnappkd.html

[S20] C：二分查找
来源：http://hz.yanxiufei.cn/gtpjqrnwlx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtphlokhkk.html

[S21] C：字符类别判断
来源：http://hz.yueranfly.top/gtrzpwjrkj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.dashuyun.cn/gtmqjohuzu.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtiathcera.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ybcxt.top/gtntwvspik.html

[S23] C：随机数
来源：http://hz.jqgfzy.top/gtnkrktpfe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xziqi.cn/gtxtibfgke.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gtaisukxyo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtzjknzils.html

[S25] C：内存拷贝
来源：http://hz.kuanghao11.cn/gtjtejrnsz.html

memcpy(dst, src, n);
来源：http://hz.cheryme.top/gtdowygtiw.html

[S26] C：内存清零
来源：http://hz.ydzc1.top/gtdgtbhhkp.html

memset(a, 0, sizeof a);
来源：http://hz.birdmap.top/gtihfcpjyk.html

[S27] C：定义常量
来源：http://hz.daxiang520.top/gtzhblikfb.html

const double PI = 3.14159;
来源：http://hz.daria6918.cn/gtrmnxmyes.html

[S28] C：静态变量
来源：http://hz.feifeiyinyue.top/gteploowvi.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtohpxosep.html

[S29] C：变参函数
来源：http://hz.shuidangran.top/gtcvqxwkwp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yangfankeji.com/gtgoxsbnbj.html

[S30] C：头文件保护
来源：http://hz.cashguo.top/gtnrbzfhwv.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtxareuuvm.html

#define X_H
来源：http://hz.zhoulong.xyz/gtablylxvd.html

#endif
来源：http://hz.shanyushiyangkeji.top/gtsbmcglmh.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gthbfhdmkv.html

#include <iostream>
来源：http://hz.dianchejie.cn/gtnbdivhaj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtigjpwohe.html

[S32] C++：字符串
来源：http://hz.guannengcc.top/gtywcnqhzn.html

std::string s = "hi";  s += "!";
来源：http://hz.cdnleiting.top/gtifirmeku.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtkyqdleoe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhaomingkeji.xyz/gtosryrfcj.html

[S34] C++：遍历 vector
来源：http://hz.ivvv.top/gtamjqgpqn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tanke756.top/gtknfycphw.html

[S35] C++：map
来源：http://hz.tanke756.top/gtgisfjvgk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtxowymgpv.html

[S36] C++：unordered_map
来源：http://hz.zhoulong.xyz/gtcgxgvmxn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtpgdxleqx.html

[S37] C++：set
来源：http://hz.jyoumei.cn/gtbdtjipre.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gttfswcbug.html

[S38] C++：排序
来源：http://hz.ywan-chungtsiang.top/gtxnjavsrp.html

std::sort(v.begin(), v.end());
来源：http://hz.yongpay.top/gtmhcwkqqz.html

[S39] C++：自定义比较器排序
来源：http://hz.gotoacloud.top/gtryejszcz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xingfuxueyuan.xyz/gtxnhpvxya.html

[S40] C++：查找元素
来源：http://hz.wangshuangyany.cn/gtoxphmtnw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgfzy.top/gtmimokoet.html

[S41] C++：类与构造函数
来源：http://hz.sufxvd.cn/gtwyukzdbn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hysaishi.cn/gtevztoqat.html

[S42] C++：继承与虚函数
来源：http://hz.zhaomingkeji.xyz/gtsjhqpizf.html

class B : public Base { public: void f() override {} };
来源：http://hz.0kj1m.cn/gtfoeznmen.html

[S43] C++：智能指针
来源：http://hz.ydzc1.top/gtrniudnse.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtejyeulre.html

[S44] C++：引用传参
来源：http://hz.zhixingplan.top/gtcmqtqdef.html

void inc(int &x) { ++x; }
来源：http://hz.sweek.top/gtufbfmqyo.html

[S45] C++：lambda
来源：http://hz.ywan-chungtsiang.top/gtcvpsgwql.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenzaomai.com/gtrldzaeqa.html

[S46] C++：函数模板
来源：http://hz.aizwys.cn/gtqvcfynwg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hysaishi.cn/gtgufnejqe.html

[S47] C++：结构化绑定遍历
来源：http://hz.quarkkingdee.top/gtonveqhxl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.316326.xyz/gtycrqegrb.html

[S48] C++：逐行读文件
来源：http://hz.wangshuangyany.cn/gtkybizmuk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgufenzy.top/gtqjqewsav.html

while (std::getline(in, line)) { }
来源：http://hz.xinyue.icu/gtedtvncyj.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtontgmska.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhixingplan.top/gtumhhjmeb.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gtoogefpop.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tanke756.top/gtuhxnnlwb.html

[S51] C++：显式类型转换
来源：http://hz.feifeiyinyue.top/gtunooiexk.html

static_cast<double>(a) / b
来源：http://hz.birdmap.top/gthslmljje.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gtpfnivqjh.html

int size() const noexcept { return n_; }
来源：http://hz.ehwqpu.com/gtzfelatxk.html

[S53] C++：移动语义
来源：http://hz.nanxinkj.top/gtgskcroco.html

std::vector<int> w = std::move(v);
来源：http://hz.zycfv.cn/gtsifzyhky.html

[S54] C++：异常处理
来源：http://hz.yongpay.top/gtbcwziboa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangdashe.top/gtstsyulwc.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtsosyurde.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtcfvkpxqd.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gttxokhneo.html


<!-- 参考信息 -->