代发 wailian999

ANALYZE TABLE users;
来源：http://hz.yj20258.top/gtzcchjwqw.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtgnbmbsik.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yueranfly.top/gtihmxnieh.html

[Q72] 查看索引
来源：http://hz.iojbl.cn/gtglqvszry.html

SHOW INDEX FROM users;
来源：http://hz.gzhubu.top/gtvpoqhuxf.html

[Q73] 查看表状态
来源：http://hz.svipenyu.cn/gtpmxlubmw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cashguo.top/gtmubkajyf.html

[Q74] 强制使用索引
来源：http://hz.ydjk.org.cn/gtretuihwg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gtprfqfreu.html

[Q75] 日期格式化
来源：http://hz.dashuyun.cn/gtxkouzgoh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhongyouzk.top/gtqkscxfdz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pycfn.com/gtxabcpoaq.html

[Q76] 按天统计
来源：http://hz.nanxinkj.top/gtkdmwuyyw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nwbrower.top/gtcmrtmnvc.html

[Q77] 时间加减
来源：http://hz.tanke756.top/gtcugvdqal.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gtxumjnjmv.html

[Q78] 当前时间
来源：http://hz.yanxiufei.cn/gtjxzzlsqw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.c1oappe.top/gtjejcfdjc.html

[Q79] 字符串拼接
来源：http://hz.yuxming.cn/gtdqlunfyr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yueranfly.top/gteqldggrq.html

[Q80] 字符串截取
来源：http://hz.havefunace.top/gthmgkhtww.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.vqdsnc.cn/gtvfwooife.html

[Q81] 字符串替换
来源：http://hz.bjfxy.top/gtzqrmgkjb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.birdmap.top/gtsxmluhqk.html

[Q82] 字符长度与字节长度
来源：http://hz.hysaishi.cn/gtwifqnryc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtbzqhbchv.html

[Q83] 大小写转换
来源：http://hz.xinyue.icu/gttaegqyth.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sufxvd.cn/gtfzbthatc.html

[Q84] 去除首尾空格
来源：http://hz.hammf.cn/gtvbowpetb.html

SELECT TRIM(name) FROM users;
来源：http://hz.yonumen.top/gtzrmaifbb.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtsnzcoclz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxuanxn.top/gtuuykktur.html

[Q86] 读取 JSON 字段
来源：http://hz.xylfe.cn/gtjhdppxmy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenjidiqi.icu/gtwdzidhho.html

[Q87] JSON 字段做条件
来源：http://hz.52xcode.cn/gtwpuombyq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cashguo.top/gttcwghydu.html

[Q88] 行转列（条件聚合）
来源：http://hz.haohaochexian.top/gtnnolaesn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenjidiqi.icu/gtnqwmuaen.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.quarkkingdee.top/gtyklyvrzd.html

[Q89] 判断表是否存在
来源：http://hz.xingfuxueyuan.xyz/gtvcrjlbje.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuxming.cn/gtncgthmno.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtkjvbdfng.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.dashuyun.cn/gtxaqfvlxo.html

================================================================================
来源：http://hz.ivvv.top/gtvxbmjvpn.html

R. Bash 专题
来源：http://hz.pycfn.com/gtoefltcxj.html

================================================================================
来源：http://hz.haohaochexian.top/gtbfcbxvfn.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gtfwhdksll.html

#!/usr/bin/env bash
来源：http://hz.nanxuanxn.top/gtkuyhtrsk.html

set -euo pipefail
来源：http://hz.cashguo.top/gtdndhjvdu.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtyzbfjilt.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtgkurfghx.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gtlmjjfizd.html

readonly PI=3.14
来源：http://hz.xingfuxueyuan.xyz/gtqcbqnmmb.html

[R04] 位置参数
来源：http://hz.gaohongyu789.top/gtuifbmcdg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cashguo.top/gtojbwmcfv.html

[R05] 参数默认值
来源：http://hz.zdqjudy.top/gtevbhfrjr.html

name="${1:-default}"
来源：http://hz.cucudq.cn/gtgzqpdiwx.html

[R06] 判断命令是否存在
来源：http://hz.316326.xyz/gtlyoqjdpy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sufxvd.cn/gtbjfptdcw.html

[R07] if 判断文件
来源：http://hz.sufxvd.cn/gtytkvlzdj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jyoumei.cn/gttpvguotc.html

[R08] 数值比较
来源：http://hz.chenzaomai.com/gtflwoztjf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtehgxbuuq.html

[R09] 字符串比较
来源：http://hz.svipenyu.cn/gtsylsyjlq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ivvv.top/gtjmcqbpin.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtbdaipqfc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yangfankeji.com/gtfzzcjygu.html

[R11] case 多分支
来源：http://hz.hammf.cn/gtbxvpckhy.html

case "$1" in
来源：http://hz.yj20258.top/gtxfklfhyq.html

start) echo "启动" ;;
来源：http://hz.hnxiangtu.top/gtlvjrzknl.html

stop)  echo "停止" ;;
来源：http://hz.yangfankeji.com/gtliheqxxi.html

*)     echo "未知命令" ;;
来源：http://hz.fzhhl.top/gtpcxhztzx.html

esac
来源：http://hz.aibaodan.cn/gtscnohaai.html

[R12] for 遍历文件
来源：http://hz.yanxiufei.cn/gtaadmvhhe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.kuanghao11.cn/gtamppqwyx.html

[R13] for 计数循环
来源：http://hz.xziqi.cn/gttxtxwnfd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtzyczaulr.html

[R14] C 风格 for
来源：http://hz.dianchejie.cn/gtgmdjjzbv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gtqsbxtuds.html

[R15] while 逐行读文件
来源：http://hz.jiagoushi.top/gtksobyyul.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.havefunace.top/gtdhtiotjh.html

[R16] until 等待条件
来源：http://hz.aizwys.cn/gtgqoghlkt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xylfe.cn/gtawsontym.html

[R17] 数组定义与取值
来源：http://hz.jqgufenzy.top/gtlnbbhkwu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangkeji.top/gtrxnsaeqw.html

[R18] 遍历数组
来源：http://hz.jyoumei.cn/gtqlxoslfx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aizwys.cn/gtxngunwxl.html

[R19] 数组长度
来源：http://hz.cdnleiting.top/gtzzpjqgaa.html

echo "${#arr[@]}"
来源：http://hz.andypj.xyz/gttpppkrmd.html

[R20] 关联数组（字典）
来源：http://hz.jqgufenzy.top/gtpnvpjgjm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shangyingyoupin.top/gtolaivbxo.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gticymmjzr.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gttoxznosc.html

[R22] 截取子串
来源：http://hz.cheryme.top/gtyyyufhru.html

echo "${s:0:5}"
来源：http://hz.vqdsnc.cn/gttngsnnui.html

[R23] 字符串替换
来源：http://hz.jinqigufen.top/gtueegxtzl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gtdecyaful.html

[R24] 大小写转换
来源：http://hz.shuidangran.top/gtnstxyihp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aizwys.cn/gtmuoqusbj.html

[R25] 去后缀 / 去前缀
来源：http://hz.shuidangran.top/gtmakyaaas.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yvedp.cn/gtoadpxsub.html

[R26] 命令替换
来源：http://hz.ivvv.top/gtuughphgj.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gteiidqosq.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gtislxylmw.html

echo $((1 + 2 * 3))
来源：http://hz.tian-w.cn/gtjergoewv.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gtvtwftndf.html

echo "scale=2; 10/3" | bc
来源：http://hz.andypj.xyz/gtvbvzpsyy.html

[R29] 定义函数
来源：http://hz.xziqi.cn/gtewcqbtak.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hywenlv.cn/gtomeejypo.html

[R30] 函数返回状态码
来源：http://hz.yuxming.cn/gtcltvprpw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuanzhike.top/gtcyqqbnvp.html

[R31] 局部变量
来源：http://hz.meibo888.top/gtxibgqupl.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtknhrtkfu.html

[R32] 参数个数校验
来源：http://hz.ppjwa.cn/gtmzeqqqna.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yonumen.top/gtjwagnxeh.html

[R33] 捕获错误并提示行号
来源：http://hz.guannengcc.top/gtvujwmwjz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.9152youxi.cn/gtuvtyfovu.html

[R34] 退出时清理
来源：http://hz.yj20258.top/gtivyhgtfp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shangyingyoupin.top/gtveczrcuk.html

[R35] 后台执行并等待
来源：http://hz.ybcxt.top/gtnchtetyu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtfgfgxtqj.html

[R36] 并发执行多个任务
来源：http://hz.gogol.net.cn/gtxfkgfrjp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tian-w.cn/gtfhjjnsyt.html

[R37] 把输出赋给变量
来源：http://hz.jiagoushi.top/gtopgfifsn.html

files=$(ls -1)
来源：http://hz.ydjk.org.cn/gtordoisbf.html

[R38] 管道串联
来源：http://hz.bjfxy.top/gtzpdwwjfx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.kuanghao11.cn/gtdddumrsx.html

[R39] 重定向标准输出与错误
来源：http://hz.ppjwa.cn/gtejhzmyzf.html

cmd > out.log 2>&1
来源：http://hz.jiagoushi.top/gtveqgypjz.html

[R40] 追加写日志
来源：http://hz.chenzaomai.com/gtkdbszwcw.html

echo "log" >> out.log
来源：http://hz.sysykeji.top/gttcbgqqam.html

[R41] 丢弃输出
来源：http://hz.zdqjudy.top/gtgkdkjvcb.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258.top/gtsbybnwii.html

[R42] 输入重定向
来源：http://hz.daxiang520.top/gtxfyyfjkg.html

wc -l < a.txt
来源：http://hz.zhiwuduotai.top/gtpoqvemvf.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gtliscnaxk.html

find . -name "*.log" -type f
来源：http://hz.snrcjt.cn/gtrmabqxal.html

[R44] 按修改时间查找
来源：http://hz.daria6918.cn/gtgvxccfey.html

find . -mtime -7 -type f
来源：http://hz.sysykeji.top/gtdmicsqqv.html

[R45] 批量删除
来源：http://hz.gaohongyu789.top/gtyubsctho.html

find . -name "*.tmp" -delete
来源：http://hz.kuanghao11.cn/gtnhveauqx.html

[R46] 递归替换文件内容
来源：http://hz.ywan-chungtsiang.top/gtgosvevmt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnxiangtu.top/gtnvweceov.html

[R47] sed 单行替换
来源：http://hz.kuanghao11.cn/gttkevgcnv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jlsjyb.cn/gtyzcympzn.html

[R48] awk 取指定列
来源：http://hz.hnxiangtu.top/gtbrrytdpo.html

awk '{print $1, $3}' a.txt
来源：http://hz.yvedp.cn/gtsshpkjha.html

[R49] awk 带条件
来源：http://hz.redwolf501.top/gtchagpfzo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenlongwang.top/gthxbdtfda.html

[R50] awk 求和
来源：http://hz.gotoacloud.top/gtpreokmea.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.meibo888.top/gtwxdnnhpe.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtoopbfohm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhiwuduotai.top/gtelgacosy.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtoytthhpx.html

wc -l a.txt
来源：http://hz.xylfe.cn/gtugglfftu.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtkrjrdgdj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zycfv.cn/gtxebccqrh.html

[R54] 比较两个文件
来源：http://hz.feifeiyinyue.top/gtfndbyfkc.html

diff a.txt b.txt
来源：http://hz.hfpthk.cn/gtrqrtxvtt.html

[R55] 压缩与解压
来源：http://hz.daxiang520.top/gtbfabmzhv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.aizwys.cn/gtriedutic.html

[R56] 远程拷贝
来源：http://hz.daxiang520.top/gtjqpolmaz.html

scp file user@host:/path/
来源：http://hz.xylfe.cn/gtnjjsjzjz.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gtwwpcjvwt.html

ssh user@host 'uptime'
来源：http://hz.ydzc1.top/gtcgxjsdgg.html

[R58] 下载文件
来源：http://hz.ywan-chungtsiang.top/gterczojfe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxuanxn.top/gttlldkvun.html

[R59] 发 POST JSON
来源：http://hz.guowangkeji.top/gtpeqlqpbb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.birdmap.top/gtqmstlvxe.html

[R60] 只看 HTTP 状态码
来源：http://hz.fzhhl.top/gtsoqaonvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hnxiangtu.top/gthupzgpmj.html

[R61] 磁盘占用
来源：http://hz.hnxiangtu.top/gtzyfbyreq.html

df -h;  du -sh *
来源：http://hz.guowangkeji.top/gtbleipkqn.html

[R62] 找最占空间的文件
来源：http://hz.yj20258888.top/gthjanboik.html

du -ah . | sort -rh | head -10
来源：http://hz.kuanghao11.cn/gtrqeadcpv.html

[R63] 内存与进程
来源：http://hz.cashguo.top/gtyglnfiaw.html

free -h;  ps aux | grep nginx
来源：http://hz.cucudq.cn/gtoruhzrbz.html

[R64] 结束进程
来源：http://hz.yvedp.cn/gtdfhljrhb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yueranfly.top/gtidfqxrnr.html

[R65] 查看端口占用
来源：http://hz.meibo888.top/gtiuyxgfkq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hywenlv.cn/gtgwrfywgz.html

[R66] 定时任务
来源：http://hz.pengpengdd.cyou/gtqmkpqqgd.html

crontab -e;  crontab -l
来源：http://hz.tianlin.xyz/gtfdxfowef.html

[R67] 生成随机十六进制串
来源：http://hz.ydzc1.top/gthvfxpmsp.html

openssl rand -hex 16
来源：http://hz.jinqigufen.top/gtktjqdere.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtbeodulst.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hysaishi.cn/gtljcbyeka.html

[R69] 生成随机密码
来源：http://hz.feifeiyinyue.top/gtepedaiok.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenjidiqi.icu/gtbasavbez.html

[R70] 时间戳与互转
来源：http://hz.aizwys.cn/gtvupuzwgg.html

date +%s;  date -d @1700000000
来源：http://hz.jqgfzy.top/gthesifhgh.html

[R71] 日期格式化
来源：http://hz.hfpthk.cn/gtghkxbdrf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pengpengdd.cyou/gtmgueixwi.html

[R72] 等待端口就绪
来源：http://hz.tian-w.cn/gtmbptwouf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guannengcc.top/gttnhrkmwm.html

[R73] 分割大日志
来源：http://hz.ydjk.org.cn/gtacifarrl.html

split -l 1000 big.log part_
来源：http://hz.ivvv.top/gtfbpkjocf.html

[R74] 批量重命名
来源：http://hz.ywan-chungtsiang.top/gttxsybzfs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hammf.cn/gtotppskhx.html

[R75] 导出环境变量
来源：http://hz.cqqwz.cn/gtidahtejm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xziqi.cn/gtuwzxmxlp.html

[R76] 使用临时文件
来源：http://hz.nwbrower.top/gtnizvwjlj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtegcsulsd.html

[R77] 读取用户输入
来源：http://hz.yuanzhike.top/gthsobcnuk.html

read -rp "请输入: " ans
来源：http://hz.hfpthk.cn/gtrcihrfur.html

[R78] 交互式菜单
来源：http://hz.gzhubu.top/gtfehtccos.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.svipenyu.cn/gthwndrgph.html

[R79] 解析命令行选项
来源：http://hz.nanxinkj.top/gtatrhsmsg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gtyvkzdwka.html

[R80] 查看脚本执行耗时
来源：http://hz.yongpay.top/gtuzqifwhx.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtpnoxhedr.html

================================================================================
来源：http://hz.cheryme.top/gtjwkuloth.html

S. C / C++ 专题
来源：http://hz.andypj.xyz/gtoeljtqbb.html

================================================================================
来源：http://hz.cdnleiting.top/gtrzgzrgvl.html

[S01] C：Hello World
来源：http://hz.mhx1999.top/gtciaigcxw.html

#include <stdio.h>
来源：http://hz.mhx1999.top/gtourjnbmf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ivvv.top/gtzzziyynh.html

[S02] C：变量与格式化输出
来源：http://hz.sufxvd.cn/gtmrloflyr.html

int a = 10; printf("%d\n", a);
来源：http://hz.hfpthk.cn/gtqniipvwr.html

[S03] C：读入整数
来源：http://hz.wangdashe.top/gtjyvllfgn.html

int x; scanf("%d", &x);
来源：http://hz.sxryk.cn/gtjqxdrbjx.html

[S04] C：字符串复制
来源：http://hz.yuxming.cn/gtrwvbdrwc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shuidangran.top/gtjvydkjmt.html

[S05] C：字符串长度
来源：http://hz.redwolf501.top/gtfywtcqgm.html

strlen(s)
来源：http://hz.birdmap.top/gtpfwtfdes.html

[S06] C：字符串比较
来源：http://hz.yj20258.top/gtljlmjdvf.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gtasqysuuw.html

[S07] C：数组遍历求和
来源：http://hz.ydjk.org.cn/gtcgnstwyu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtwamkusjp.html

[S08] C：动态内存分配与释放
来源：http://hz.gogol.net.cn/gtyjbycprf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yvedp.cn/gtncwtwesx.html

[S09] C：结构体定义与初始化
来源：http://hz.shangyingyoupin.top/gtfydozmbx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shangyingyoupin.top/gthhzinfgu.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtoegfnpbr.html

int *p = &a;  *p = 5;
来源：http://hz.xinyue.icu/gtbqjlqokx.html

[S11] C：逐行读文件
来源：http://hz.aizwys.cn/gtcoheifxl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.kuanghao11.cn/gtctjyauer.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenzaomai.com/gtfmyhwtkq.html

fclose(f);
来源：http://hz.gogol.net.cn/gtofxmietr.html

[S12] C：写文件
来源：http://hz.nwbrower.top/gttyswcnos.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tianlin.xyz/gtqtseubaq.html

[S13] C：宏定义
来源：http://hz.gogol.net.cn/gttkyajchr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dashuyun.cn/gtdosngxld.html

[S14] C：枚举
来源：http://hz.smart0.xyz/gtlevtjvxp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuetiantiany.cn/gteongfbkr.html

[S15] C：类型转换
来源：http://hz.tanke756.top/gtehdudgqn.html

(double) a / b
来源：http://hz.xuetiantiany.cn/gtyslzzfik.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtzlpsiznh.html

x |= (1 << 3);
来源：http://hz.shanyushiyangkeji.top/gtbuydhaml.html

[S17] C：安全拼接字符串
来源：http://hz.hnxiangtu.top/gtflefoeyz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pengpengdd.cyou/gtggpydojp.html

[S18] C：命令行参数
来源：http://hz.cheryme.top/gtpnmvumnn.html

int main(int argc, char **argv)
来源：http://hz.cheryme.top/gtexyjbiey.html

[S19] C：快速排序
来源：http://hz.hywenlv.cn/gtmqfosfkt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtyoyqouip.html

[S20] C：二分查找
来源：http://hz.feifeiyinyue.top/gtislzkvtl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtmfjyqvpf.html

[S21] C：字符类别判断
来源：http://hz.yueranfly.top/gtikzmthez.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhijiandao.cn/gtrapoatvg.html

[S22] C：字符串转数字
来源：http://hz.nanxinkj.top/gtjqqhradk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dashuyun.cn/gtdtzrpbss.html

[S23] C：随机数
来源：http://hz.wangshuangyany.cn/gtdmjommpg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtggfmmgno.html

[S24] C：获取本地时间
来源：http://hz.kuanghao11.cn/gtbuyxddke.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aizwys.cn/gtztkhjspa.html

[S25] C：内存拷贝
来源：http://hz.cucudq.cn/gtwdsaohlp.html

memcpy(dst, src, n);
来源：http://hz.jinyuanbaomall.cn/gtejkywzif.html

[S26] C：内存清零
来源：http://hz.hywenlv.cn/gtspgrnfyz.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gthjjiuzmn.html

[S27] C：定义常量
来源：http://hz.chenlongwang.top/gtgfyhoavx.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtchgcqcax.html

[S28] C：静态变量
来源：http://hz.yangfankeji.com/gtdgtscviv.html

static int counter = 0;
来源：http://hz.ehwqpu.com/gtofogwwrs.html

[S29] C：变参函数
来源：http://hz.hnxiangtu.top/gtbrsgaspg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jlsjyb.cn/gtloxnefdr.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtnbylnscq.html

#ifndef X_H
来源：http://hz.jianghu66.top/gtypwkbgys.html

#define X_H
来源：http://hz.pycfn.com/gtvlhcsblm.html

#endif
来源：http://hz.shangyingyoupin.top/gtuzjzehtp.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtnvqdcqtv.html

#include <iostream>
来源：http://hz.nwbrower.top/gtmhmoiiqe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daxiang520.top/gtonswobjd.html

[S32] C++：字符串
来源：http://hz.ehwqpu.com/gthfisanoh.html

std::string s = "hi";  s += "!";
来源：http://hz.zycfv.cn/gtdffdowgc.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtpfzstfmn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daria6918.cn/gtgqaqiyvq.html

[S34] C++：遍历 vector
来源：http://hz.xinyue.icu/gtjqcnfmpt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yangfankeji.com/gtnetqairz.html

[S35] C++：map
来源：http://hz.hammf.cn/gtnxnrmtsc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ppjwa.cn/gthhzsvprj.html

[S36] C++：unordered_map
来源：http://hz.0kj1m.cn/gtnorhexja.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtfmkexstw.html

[S37] C++：set
来源：http://hz.shuidangran.top/gtvsayjzim.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtobcxyouf.html

[S38] C++：排序
来源：http://hz.aizwys.cn/gtjksyszdr.html

std::sort(v.begin(), v.end());
来源：http://hz.zhijiandao.cn/gtommwsiph.html

[S39] C++：自定义比较器排序
来源：http://hz.cashguo.top/gtqfajnrab.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dianchejie.cn/gtmxgnrlgv.html

[S40] C++：查找元素
来源：http://hz.yangfankeji.com/gthgvrhzii.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hywenlv.cn/gtvrquazhr.html


<!-- 参考信息 -->