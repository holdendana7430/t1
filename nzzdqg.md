代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.hammf.cn/gtqapgbuez.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sxryk.cn/gtdppvoyae.html

[Q83] 大小写转换
来源：http://hz.jlsjyb.cn/gtecmoqpaw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxinkj.top/gtcdzfbyui.html

[Q84] 去除首尾空格
来源：http://hz.zhongyouzk.top/gtzhyzuyiu.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuxming.cn/gtgpfnjmwz.html

[Q85] 数值取整
来源：http://hz.feifeiyinyue.top/gtksezsvsn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gtfqtnhcfq.html

[Q86] 读取 JSON 字段
来源：http://hz.zycfv.cn/gtypxeadea.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangdashe.top/gtftaqtquw.html

[Q87] JSON 字段做条件
来源：http://hz.sysykeji.top/gtoecootol.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tianlin.xyz/gthjkkcipq.html

[Q88] 行转列（条件聚合）
来源：http://hz.havefunace.top/gtvxzubwxr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guowangkeji.top/gttjwptfvg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxinkj.top/gtslfqzbca.html

[Q89] 判断表是否存在
来源：http://hz.chenzaomai.com/gtixyirsem.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.meibo888.top/gtktudlqrn.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtksmjqtks.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuanzhike.top/gtxaqyrfkr.html

================================================================================
来源：http://hz.jinqigufen.top/gtzhkbyeht.html

R. Bash 专题
来源：http://hz.hnxiangtu.top/gtzdrrazxg.html

================================================================================
来源：http://hz.birdmap.top/gtmkwuodpt.html

[R01] shebang 与严格模式
来源：http://hz.fengsongda.top/gtfdawomiy.html

#!/usr/bin/env bash
来源：http://hz.cqqwz.cn/gtfoqzphrn.html

set -euo pipefail
来源：http://hz.hammf.cn/gtacfazyhl.html

[R02] 变量赋值与使用
来源：http://hz.cdnleiting.top/gtskeohnui.html

name="Tom"; echo "$name"
来源：http://hz.haohaochexian.top/gtotpwwktu.html

[R03] 只读变量
来源：http://hz.yonumen.top/gtkhcolwtn.html

readonly PI=3.14
来源：http://hz.iojbl.cn/gtdaisnjki.html

[R04] 位置参数
来源：http://hz.xinyue.icu/gtiqoeeftj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hywenlv.cn/gtyuhqudfz.html

[R05] 参数默认值
来源：http://hz.zhoulong.xyz/gtqagdlqqv.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtbtoxssah.html

[R06] 判断命令是否存在
来源：http://hz.chenzaomai.com/gtsxmbkswp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yonumen.top/gtkckcweij.html

[R07] if 判断文件
来源：http://hz.yvedp.cn/gtbcqjyxdy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jqgufenzy.top/gtnfdpejou.html

[R08] 数值比较
来源：http://hz.jqgufenzy.top/gtrhhvuknc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigufen.top/gtlpmrwmol.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gttqvbgglf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuetiantiany.cn/gtgbgglfac.html

[R10] 正则匹配
来源：http://hz.xuanzx.com/gtdxgrqmuf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dashuyun.cn/gtvwvlazjf.html

[R11] case 多分支
来源：http://hz.iojbl.cn/gtyfcjxibf.html

case "$1" in
来源：http://hz.sweek.top/gtcetkfghy.html

start) echo "启动" ;;
来源：http://hz.xingfuxueyuan.xyz/gtadhmkvqz.html

stop)  echo "停止" ;;
来源：http://hz.guannengcc.top/gtiqjadzas.html

*)     echo "未知命令" ;;
来源：http://hz.haohaochexian.top/gtmumntjck.html

esac
来源：http://hz.chenlongwang.top/gtjnlwfyta.html

[R12] for 遍历文件
来源：http://hz.jinghuilouyu.cn/gtttkgrxfp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtsrtqimuw.html

[R13] for 计数循环
来源：http://hz.cucudq.cn/gtvifqsvul.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtwxpeuuef.html

[R14] C 风格 for
来源：http://hz.xingfuxueyuan.xyz/gtjyvgewus.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtbijhdogx.html

[R15] while 逐行读文件
来源：http://hz.hnxiangtu.top/gtunusagaf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.52xcode.cn/gtdszdykkg.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gthsmcthlb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gzhubu.top/gtfxmndbtj.html

[R17] 数组定义与取值
来源：http://hz.jinghuilouyu.cn/gtqwpuupke.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangshuangyany.cn/gtqfxkxhvd.html

[R18] 遍历数组
来源：http://hz.vqdsnc.cn/gtudfflbox.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtrlvaaixa.html

[R19] 数组长度
来源：http://hz.chenlongwang.top/gtrrlonttn.html

echo "${#arr[@]}"
来源：http://hz.hnqzz.top/gtkgopzmie.html

[R20] 关联数组（字典）
来源：http://hz.ybcxt.top/gtysbvuyir.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jiagoushi.top/gthycfifvl.html

[R21] 字符串长度
来源：http://hz.sxryk.cn/gtroarwkqg.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtecqbcasv.html

[R22] 截取子串
来源：http://hz.haohaochexian.top/gtommwkkow.html

echo "${s:0:5}"
来源：http://hz.yueranfly.top/gtylkmheto.html

[R23] 字符串替换
来源：http://hz.zhongyouzk.top/gtfrhkrqqm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinghuilouyu.cn/gtvqgpxvaz.html

[R24] 大小写转换
来源：http://hz.shzxlz.cn/gtkyvszdvd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ybcxt.top/gtgujacqrf.html

[R25] 去后缀 / 去前缀
来源：http://hz.smart0.xyz/gtovjicboq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hfpthk.cn/gttwoschxv.html

[R26] 命令替换
来源：http://hz.snrcjt.cn/gtewqdvbny.html

now=$(date +%F); echo "$now"
来源：http://hz.zhoulong.xyz/gtacjphxqy.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtkfvllqmm.html

echo $((1 + 2 * 3))
来源：http://hz.gaohongyu789.top/gtvffcfrzp.html

[R28] 浮点运算
来源：http://hz.havefunace.top/gtamzpsjmm.html

echo "scale=2; 10/3" | bc
来源：http://hz.dianchejie.cn/gtxuqjpgbx.html

[R29] 定义函数
来源：http://hz.jinqigufen.top/gtfpbqgwgs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xingfuxueyuan.xyz/gtcimhfhrn.html

[R30] 函数返回状态码
来源：http://hz.316326.xyz/gtthessyyb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gotoacloud.top/gttihjlqyg.html

[R31] 局部变量
来源：http://hz.jiagoushi.top/gtheqsttou.html

f() { local x=1; echo "$x"; }
来源：http://hz.shuidangran.top/gtkzjjszhg.html

[R32] 参数个数校验
来源：http://hz.gzhubu.top/gthmgfpzfp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigfzy.top/gtmuyqpotd.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtmntpusyq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangdashe.top/gtwsixssrt.html

[R34] 退出时清理
来源：http://hz.havefunace.top/gthdklsxpw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtbsrexbpi.html

[R35] 后台执行并等待
来源：http://hz.yueranfly.top/gthqyxgeph.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtiwgkviam.html

[R36] 并发执行多个任务
来源：http://hz.pengpengdd.cyou/gthcypcnuq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gtrqvmvlaa.html

[R37] 把输出赋给变量
来源：http://hz.quarkkingdee.top/gtfzarwkbo.html

files=$(ls -1)
来源：http://hz.xuanzx.com/gtjevzpfnd.html

[R38] 管道串联
来源：http://hz.zycfv.cn/gtnelkisya.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtjfckqiaz.html

[R39] 重定向标准输出与错误
来源：http://hz.jlsjyb.cn/gtcnthdggo.html

cmd > out.log 2>&1
来源：http://hz.xinyue.icu/gthqmmupup.html

[R40] 追加写日志
来源：http://hz.snrcjt.cn/gtfxulssku.html

echo "log" >> out.log
来源：http://hz.jinyuanbaomall.cn/gtycatuwce.html

[R41] 丢弃输出
来源：http://hz.ivvv.top/gtqcuiserq.html

cmd >/dev/null 2>&1
来源：http://hz.sweek.top/gtezqwlxvo.html

[R42] 输入重定向
来源：http://hz.cashguo.top/gtqukgjmat.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtybxumlez.html

[R43] 按名字查找文件
来源：http://hz.yangfankeji.com/gthpftenac.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gtrohhwhow.html

[R44] 按修改时间查找
来源：http://hz.jianghu66.top/gtsdanesgm.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtrogdyizv.html

[R45] 批量删除
来源：http://hz.xingfuxueyuan.xyz/gtvisowzpj.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtvlottkrg.html

[R46] 递归替换文件内容
来源：http://hz.yj202588.top/gtbvgeqkfg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtlwhzeywh.html

[R47] sed 单行替换
来源：http://hz.jinqigfzy.top/gtemswqgay.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.9152youxi.cn/gtesdraaux.html

[R48] awk 取指定列
来源：http://hz.jinqigfzy.top/gtkeieukuy.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgufenzy.top/gtulfptsxv.html

[R49] awk 带条件
来源：http://hz.iojbl.cn/gtyzojlthu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.316326.xyz/gtyclarodg.html

[R50] awk 求和
来源：http://hz.hysaishi.cn/gtaeljhqik.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhongyouzk.top/gtjjhjwmgl.html

[R51] 排序去重取前几
来源：http://hz.andypj.xyz/gteqvykfob.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenjidiqi.icu/gtwqzzeygc.html

[R52] 统计行数
来源：http://hz.xylfe.cn/gtnpzcttxv.html

wc -l a.txt
来源：http://hz.hnqzz.top/gtuvkyfepx.html

[R53] 查看文件头与实时尾
来源：http://hz.redwolf501.top/gtjiwoewlr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtulpbshnf.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtogkhuqwb.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gtnzwyqhhh.html

[R55] 压缩与解压
来源：http://hz.bjfxy.top/gtpfkwljjm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hywenlv.cn/gtelkfpqet.html

[R56] 远程拷贝
来源：http://hz.dashuyun.cn/gtesrqcgym.html

scp file user@host:/path/
来源：http://hz.ywan-chungtsiang.top/gtereyijgv.html

[R57] 远程执行命令
来源：http://hz.yuanzhike.top/gtvkmvrxku.html

ssh user@host 'uptime'
来源：http://hz.jqgufenzy.top/gtojfultuy.html

[R58] 下载文件
来源：http://hz.0kj1m.cn/gtaorivnef.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtkistfvuk.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtjzpaajiz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gtzepgmbgh.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gtucdahhex.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtwejifsxw.html

[R61] 磁盘占用
来源：http://hz.sufxvd.cn/gtisanfawu.html

df -h;  du -sh *
来源：http://hz.c1oappe.top/gtbtpmhnnn.html

[R62] 找最占空间的文件
来源：http://hz.jinghuilouyu.cn/gtwlkzivkz.html

du -ah . | sort -rh | head -10
来源：http://hz.cashguo.top/gtflpswsgd.html

[R63] 内存与进程
来源：http://hz.guannengcc.top/gtbbnitmsn.html

free -h;  ps aux | grep nginx
来源：http://hz.cucudq.cn/gthmbzndhk.html

[R64] 结束进程
来源：http://hz.bjfxy.top/gttmkfnpbv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cucudq.cn/gtesvgvbtk.html

[R65] 查看端口占用
来源：http://hz.hongshengwenyu.top/gtfbrgopgv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigfzy.top/gthzxpnftn.html

[R66] 定时任务
来源：http://hz.wangshuangyany.cn/gtkaziwzhp.html

crontab -e;  crontab -l
来源：http://hz.yueranfly.top/gtjjcyywul.html

[R67] 生成随机十六进制串
来源：http://hz.dashuyun.cn/gtukdidynz.html

openssl rand -hex 16
来源：http://hz.pengpengdd.cyou/gtgiugbbuz.html

[R68] 计算文件校验值
来源：http://hz.birdmap.top/gthtvqamda.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtqxyggjct.html

[R69] 生成随机密码
来源：http://hz.yj20258888.top/gtyhpspxis.html

head -c 16 /dev/urandom | base64
来源：http://hz.gaohongyu789.top/gtsbevglgh.html

[R70] 时间戳与互转
来源：http://hz.tianlin.xyz/gtfroutddj.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtuvlohpnc.html

[R71] 日期格式化
来源：http://hz.zycfv.cn/gtqvucmwhw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtuqssztzu.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gtffbgfjnc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xinyue.icu/gtbnowmbfr.html

[R73] 分割大日志
来源：http://hz.jinghuilouyu.cn/gtfccwrzmu.html

split -l 1000 big.log part_
来源：http://hz.xingfuxueyuan.xyz/gtpzlnbkqd.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtajddrrlt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gtwsftlnmz.html

[R75] 导出环境变量
来源：http://hz.aibaodan.cn/gtlxefcmqq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gtbfabcyhp.html

[R76] 使用临时文件
来源：http://hz.sxryk.cn/gtddueyqkt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtsbpvkfis.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtfuqhzljm.html

read -rp "请输入: " ans
来源：http://hz.ybcxt.top/gtnlxggvau.html

[R78] 交互式菜单
来源：http://hz.zdqjudy.top/gtoqswrnnz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.havefunace.top/gtecukxpop.html

[R79] 解析命令行选项
来源：http://hz.sxryk.cn/gtqrpewkus.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gtimfqbdxa.html

[R80] 查看脚本执行耗时
来源：http://hz.gogol.net.cn/gtdictryka.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtovpcngyg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtcvzilasa.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtgbvciyye.html

================================================================================
来源：http://hz.yj20258888.top/gtmbgumlij.html

[S01] C：Hello World
来源：http://hz.wangdashe.top/gtosgoitjl.html

#include <stdio.h>
来源：http://hz.jiagoushi.top/gtsqvhsihf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhixingplan.top/gtcipglrwm.html

[S02] C：变量与格式化输出
来源：http://hz.jqgfzy.top/gtqcstvmnd.html

int a = 10; printf("%d\n", a);
来源：http://hz.aibaodan.cn/gtmaqwfigb.html

[S03] C：读入整数
来源：http://hz.gzhubu.top/gtiarfdaye.html

int x; scanf("%d", &x);
来源：http://hz.snrcjt.cn/gtwgjchdpl.html

[S04] C：字符串复制
来源：http://hz.andypj.xyz/gtrmxkzevw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ywan-chungtsiang.top/gtmvtqppkd.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtqxztjwab.html

strlen(s)
来源：http://hz.cdnleiting.top/gtlfhcgmmd.html

[S06] C：字符串比较
来源：http://hz.yuxming.cn/gtatpxcfrj.html

strcmp(a, b) == 0
来源：http://hz.gogol.net.cn/gtelnefpft.html

[S07] C：数组遍历求和
来源：http://hz.svipenyu.cn/gtqrpjzdre.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sweek.top/gtiflmecfo.html

[S08] C：动态内存分配与释放
来源：http://hz.cheryme.top/gtibyhtgto.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtirxuolsy.html

[S09] C：结构体定义与初始化
来源：http://hz.mhx1999.top/gtzievjycx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nanxuanxn.top/gturyspmjd.html

[S10] C：指针与解引用
来源：http://hz.birdmap.top/gtqusyrhuo.html

int *p = &a;  *p = 5;
来源：http://hz.52xcode.cn/gtywlrogkr.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtsydkytha.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtibhhoisb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ivvv.top/gtskxjyelu.html

fclose(f);
来源：http://hz.xuetiantiany.cn/gtlgnpdpjv.html

[S12] C：写文件
来源：http://hz.feifeiyinyue.top/gttdxpfqgw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258888.top/gtmqyaimtu.html

[S13] C：宏定义
来源：http://hz.dianchejie.cn/gtbirwybjj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pengpengdd.cyou/gtlnzewuvi.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtmuwehjkt.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gtratzthfw.html

[S15] C：类型转换
来源：http://hz.zhongyouzk.top/gtqouaytmp.html

(double) a / b
来源：http://hz.havefunace.top/gtequygqis.html

[S16] C：位操作置位
来源：http://hz.hfpthk.cn/gtcghucjax.html

x |= (1 << 3);
来源：http://hz.guowangkeji.top/gtfnfvbjpf.html

[S17] C：安全拼接字符串
来源：http://hz.vqdsnc.cn/gtdipeqqod.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnxiangtu.top/gtiwtlhayq.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtegquirzj.html

int main(int argc, char **argv)
来源：http://hz.snrcjt.cn/gtnrzjjceu.html

[S19] C：快速排序
来源：http://hz.tianlin.xyz/gtlwikgild.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtyohtwqar.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtookkpnhr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtpnjjmysm.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gthtjyridi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gaohongyu789.top/gtcwgmhvrg.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtmevhgyrj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sweek.top/gtsjowhfmu.html

[S23] C：随机数
来源：http://hz.yangfankeji.com/gthvgwzrdl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gtrrwpktke.html

[S24] C：获取本地时间
来源：http://hz.jinqigfzy.top/gtldwrnfji.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cucudq.cn/gtedkjrohf.html

[S25] C：内存拷贝
来源：http://hz.ehwqpu.com/gtlznionjz.html

memcpy(dst, src, n);
来源：http://hz.fengsongda.top/gtakxatipg.html

[S26] C：内存清零
来源：http://hz.iojbl.cn/gtxhqbxbng.html

memset(a, 0, sizeof a);
来源：http://hz.xuetiantiany.cn/gtxkrvietc.html

[S27] C：定义常量
来源：http://hz.yongpay.top/gtezroumwp.html

const double PI = 3.14159;
来源：http://hz.meibo888.top/gtdltiafvf.html

[S28] C：静态变量
来源：http://hz.sufxvd.cn/gtgxaeozdh.html

static int counter = 0;
来源：http://hz.316326.xyz/gtcrwyadkm.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gthjroqzxo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtkdpyizfb.html

[S30] C：头文件保护
来源：http://hz.ehwqpu.com/gtbmscbilu.html

#ifndef X_H
来源：http://hz.xuanzx.com/gtlholpsyf.html

#define X_H
来源：http://hz.ppjwa.cn/gtuaggxbrg.html

#endif
来源：http://hz.tianlin.xyz/gtyqagyocx.html

[S31] C++：Hello World
来源：http://hz.jyoumei.cn/gtowixsoli.html

#include <iostream>
来源：http://hz.nwbrower.top/gtvokxnldh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.kuanghao11.cn/gtmandqunm.html

[S32] C++：字符串
来源：http://hz.shanyushiyangkeji.top/gtzitwswkv.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangtech.top/gtlabmmqtc.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gtphauumfq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.kuanghao11.cn/gtmuuahntk.html

[S34] C++：遍历 vector
来源：http://hz.nanxinkj.top/gtvfxphfzk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.haohaochexian.top/gthzcawwjg.html

[S35] C++：map
来源：http://hz.xziqi.cn/gtneawrvyp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtivggjyvt.html

[S36] C++：unordered_map
来源：http://hz.ywan-chungtsiang.top/gtjopmezme.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daria6918.cn/gtzetvqbtb.html

[S37] C++：set
来源：http://hz.52xcode.cn/gtpclcchpk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cheryme.top/gtwlysfqbf.html

[S38] C++：排序
来源：http://hz.jiagoushi.top/gtkriywzzp.html

std::sort(v.begin(), v.end());
来源：http://hz.ybcxt.top/gtbexfpweo.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigufen.top/gtsvxvajfw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daria6918.cn/gtaxkkjhtp.html

[S40] C++：查找元素
来源：http://hz.shangyingyoupin.top/gtvyipduet.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenlongwang.top/gtwucgobrz.html

[S41] C++：类与构造函数
来源：http://hz.ybcxt.top/gtmhzzyfff.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.52xcode.cn/gtfzakbrfb.html

[S42] C++：继承与虚函数
来源：http://hz.shanyushiyangkeji.top/gtsfzujmtb.html

class B : public Base { public: void f() override {} };
来源：http://hz.xziqi.cn/gtigmpiucu.html

[S43] C++：智能指针
来源：http://hz.0kj1m.cn/gtffhtqmbj.html

auto p = std::make_unique<int>(5);
来源：http://hz.yueranfly.top/gtwziitbxh.html

[S44] C++：引用传参
来源：http://hz.ywan-chungtsiang.top/gtlbqvsixb.html

void inc(int &x) { ++x; }
来源：http://hz.zhongyouzk.top/gticgodvpe.html

[S45] C++：lambda
来源：http://hz.jinyuanbaomall.cn/gtcyczcidd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gogol.net.cn/gtvcncarek.html

[S46] C++：函数模板
来源：http://hz.nanxuanxn.top/gtwllwjwmn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinyuanbaomall.cn/gtcwzceejd.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtozmqfczp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhiwuduotai.top/gtcoblqxnt.html

[S48] C++：逐行读文件
来源：http://hz.sweek.top/gtpsfjfnwz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.guannengcc.top/gtkxdrwpyd.html

while (std::getline(in, line)) { }
来源：http://hz.jiagoushi.top/gtuvfebgyp.html

[S49] C++：写文件
来源：http://hz.hfpthk.cn/gtttdrgytd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guannengcc.top/gtoydtkfpn.html

[S50] C++：格式化数字
来源：http://hz.fzhhl.top/gtawwcbnbj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.svipenyu.cn/gtmvxytjdj.html

[S51] C++：显式类型转换
来源：http://hz.haohaochexian.top/gtvduufefr.html

static_cast<double>(a) / b
来源：http://hz.cdnleiting.top/gtoeneaorj.html

[S52] C++：const 与 noexcept
来源：http://hz.hysaishi.cn/gtryhowudv.html


<!-- 参考信息 -->