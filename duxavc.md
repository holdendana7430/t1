代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xziqi.cn/gtowvbddhg.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtcbycvxyq.html

TRUNCATE TABLE logs;
来源：http://hz.9152youxi.cn/gtivqflzle.html

[Q55] 排名（并列占位）
来源：http://hz.chenjidiqi.icu/gtdamfeuap.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxuanxn.top/gtaxmwjgqb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shangyingyoupin.top/gthvztvtwp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hnxiangtu.top/gtvcypluyg.html

[Q57] 行号
来源：http://hz.ppjwa.cn/gtvctijtxa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtgmkxxttm.html

[Q58] 累计求和
来源：http://hz.ppjwa.cn/gtnvkpiduw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guowangkeji.top/gtvziceqkk.html

[Q59] 分组内累计
来源：http://hz.hongshengwenyu.top/gtmkyuhdsi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtmezrellb.html

[Q60] 取上一行 / 下一行
来源：http://hz.aibaodan.cn/gteznjuowi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xinyue.icu/gtvlgdvnwm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fengsongda.top/gtroondokw.html

[Q61] 移动平均
来源：http://hz.jiagoushi.top/gtfdpqfnbu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ybcxt.top/gtvlbyabgo.html

[Q62] 分组占比
来源：http://hz.ehwqpu.com/gtamlsnktu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtdzcvhlza.html

[Q63] 开启事务
来源：http://hz.jiagoushi.top/gtmlwqrkmb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtrljacmgz.html

[Q64] 提交事务
来源：http://hz.xziqi.cn/gtztwpnqoz.html

COMMIT;
来源：http://hz.ydjk.org.cn/gtbwipstzb.html

[Q65] 回滚事务
来源：http://hz.jinyuanbaomall.cn/gtqfcnjvap.html

ROLLBACK;
来源：http://hz.jqgfzy.top/gttgrfeawr.html

[Q66] 行锁查询
来源：http://hz.ivvv.top/gtqsjghxrb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hysaishi.cn/gtbjyhfvqo.html

[Q67] 设置隔离级别
来源：http://hz.ybcxt.top/gtutzbwvbi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hysaishi.cn/gtwvzudkkf.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtrxpdfwvh.html

SAVEPOINT sp1;
来源：http://hz.hongshengwenyu.top/gtyqrstjph.html

ROLLBACK TO sp1;
来源：http://hz.tanke756.top/gtcfjxkrkd.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtczxisloj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.smart0.xyz/gtnqwfbmuj.html

[Q70] 更新统计信息
来源：http://hz.jinqigufen.top/gtmsrqrkoa.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtkntijddn.html

[Q71] 查看建表语句
来源：http://hz.zhengqikj.top/gttyffvkli.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.bjfxy.top/gtswvemtvd.html

[Q72] 查看索引
来源：http://hz.vqdsnc.cn/gtbhmldciz.html

SHOW INDEX FROM users;
来源：http://hz.svipenyu.cn/gtcelgqwpu.html

[Q73] 查看表状态
来源：http://hz.smart0.xyz/gtcruymyad.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xinyue.icu/gtxvxrzvza.html

[Q74] 强制使用索引
来源：http://hz.ppjwa.cn/gtihiikowu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258.top/gtsvwojbsn.html

[Q75] 日期格式化
来源：http://hz.sysykeji.top/gtjnspraxg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cheryme.top/gtdupxflkx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shuidangran.top/gthygxbwrf.html

[Q76] 按天统计
来源：http://hz.ivvv.top/gtzkmnliqc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jqgfzy.top/gtpuemzixy.html

[Q77] 时间加减
来源：http://hz.sysykeji.top/gtlaurswzj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ywan-chungtsiang.top/gtplawgozx.html

[Q78] 当前时间
来源：http://hz.sxryk.cn/gtcxwvyamf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ivvv.top/gtpmqzfgef.html

[Q79] 字符串拼接
来源：http://hz.nwbrower.top/gtdmcyvovl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yangfankeji.com/gtxixrtkbs.html

[Q80] 字符串截取
来源：http://hz.havefunace.top/gtizbrqnsc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tian-w.cn/gtxprnzwdi.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtpqtwsftj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgufenzy.top/gtncshkzpp.html

[Q82] 字符长度与字节长度
来源：http://hz.havefunace.top/gtzfgpllyk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cdnleiting.top/gtwecsdgdb.html

[Q83] 大小写转换
来源：http://hz.fengsongda.top/gtwydopuvz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydzc1.top/gtfkidflpk.html

[Q84] 去除首尾空格
来源：http://hz.wangdashe.top/gttsdmkvya.html

SELECT TRIM(name) FROM users;
来源：http://hz.kuanghao11.cn/gtxhwxblxi.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gtwaoofwsr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gtjnqfjjzv.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxinkj.top/gtfojxzmtk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigfzy.top/gtmlrftpnw.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258888.top/gtvdsmaqpf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jyoumei.cn/gtpitnmtcs.html

[Q88] 行转列（条件聚合）
来源：http://hz.cucudq.cn/gtnrnpguki.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigufen.top/gtviptboui.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.snrcjt.cn/gtxypikzky.html

[Q89] 判断表是否存在
来源：http://hz.snrcjt.cn/gtqgcarads.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtbbrnbmji.html

[Q90] 生成序号列
来源：http://hz.gaohongyu789.top/gtlvtaiimc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gaohongyu789.top/gtirmfxuom.html

================================================================================
来源：http://hz.tian-w.cn/gtjdqndzdj.html

R. Bash 专题
来源：http://hz.aizwys.cn/gtbvlaheoh.html

================================================================================
来源：http://hz.redwolf501.top/gtygqjnsns.html

[R01] shebang 与严格模式
来源：http://hz.c1oappe.top/gtbafqovzl.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtzpuyjrxp.html

set -euo pipefail
来源：http://hz.pycfn.com/gtklmnhroq.html

[R02] 变量赋值与使用
来源：http://hz.zhaomingkeji.xyz/gtsymfegwk.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gttbbakrhq.html

[R03] 只读变量
来源：http://hz.cashguo.top/gtragbqnbi.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gttwgmbdrh.html

[R04] 位置参数
来源：http://hz.iojbl.cn/gtqcqsxuui.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtojwgtrkz.html

[R05] 参数默认值
来源：http://hz.0kj1m.cn/gtutzmvyze.html

name="${1:-default}"
来源：http://hz.shanyushiyangkeji.top/gttcxdqtsp.html

[R06] 判断命令是否存在
来源：http://hz.zhongyouzk.top/gtinbxclin.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sweek.top/gteiojsynm.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtemtfetyh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daria6918.cn/gtqsqxybui.html

[R08] 数值比较
来源：http://hz.pengpengdd.cyou/gtepuplwfj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhiwuduotai.top/gtzbcsquja.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gtwxhraddz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.mhx1999.top/gtxplewjhi.html

[R10] 正则匹配
来源：http://hz.tian-w.cn/gtoucyudud.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nwbrower.top/gtrdrzpsfv.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtzoihdlmw.html

case "$1" in
来源：http://hz.0kj1m.cn/gthozsdxzf.html

start) echo "启动" ;;
来源：http://hz.jyoumei.cn/gtfvlrbuwe.html

stop)  echo "停止" ;;
来源：http://hz.fengsongda.top/gtfvmgmsyo.html

*)     echo "未知命令" ;;
来源：http://hz.cdnleiting.top/gtieffgswj.html

esac
来源：http://hz.yangfankeji.com/gtmnpgihps.html

[R12] for 遍历文件
来源：http://hz.hfpthk.cn/gtqsxsrtsh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gtllxjgdda.html

[R13] for 计数循环
来源：http://hz.yongpay.top/gtbwbabrqt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.svipenyu.cn/gtswuzjpuv.html

[R14] C 风格 for
来源：http://hz.zhengqikj.top/gtezoknwok.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.smart0.xyz/gtaibdkflq.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtyvdtmsiu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtliluoszn.html

[R16] until 等待条件
来源：http://hz.yongpay.top/gteqslusuh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hammf.cn/gtfcmgtfhi.html

[R17] 数组定义与取值
来源：http://hz.316326.xyz/gtnsoamgpq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhongyouzk.top/gtgohmuqzz.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gtdtnjmzdh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhoulong.xyz/gtwctxuuvn.html

[R19] 数组长度
来源：http://hz.yvedp.cn/gtznexuwfc.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtrxuqelmy.html

[R20] 关联数组（字典）
来源：http://hz.vqdsnc.cn/gtiznuwmdo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigfzy.top/gtbgkxhpyi.html

[R21] 字符串长度
来源：http://hz.ywan-chungtsiang.top/gtgwxnjasw.html

echo "${#s}"
来源：http://hz.ivvv.top/gtwhsxtvai.html

[R22] 截取子串
来源：http://hz.aizwys.cn/gtaazvdjbr.html

echo "${s:0:5}"
来源：http://hz.dianchejie.cn/gtdyzumxrs.html

[R23] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtkyycgqyg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gtblzuewqd.html

[R24] 大小写转换
来源：http://hz.gogol.net.cn/gtrhuquutg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258.top/gtjwtyavuo.html

[R25] 去后缀 / 去前缀
来源：http://hz.yongpay.top/gtxtkiryip.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigufen.top/gtrymausbj.html

[R26] 命令替换
来源：http://hz.ybcxt.top/gtfwtilygv.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtxoeuvqsq.html

[R27] 算术展开
来源：http://hz.shzxlz.cn/gtictktrak.html

echo $((1 + 2 * 3))
来源：http://hz.nanxinkj.top/gtoxbhwhiu.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtymvrfdga.html

echo "scale=2; 10/3" | bc
来源：http://hz.pengpengdd.cyou/gtlcampspb.html

[R29] 定义函数
来源：http://hz.bjfxy.top/gtmxpkrimz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtzsgkzdls.html

[R30] 函数返回状态码
来源：http://hz.0kj1m.cn/gtkbgjaqlz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.redwolf501.top/gtscxavyqw.html

[R31] 局部变量
来源：http://hz.pycfn.com/gtymnohbzg.html

f() { local x=1; echo "$x"; }
来源：http://hz.svipenyu.cn/gtzvufwcbf.html

[R32] 参数个数校验
来源：http://hz.cheryme.top/gtlaxqoniq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guowangkeji.top/gtabidfvon.html

[R33] 捕获错误并提示行号
来源：http://hz.yangfankeji.com/gtxfdsnqyc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.feifeiyinyue.top/gtqelzxzkp.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gtmeyhokjs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtnfnfiwfg.html

[R35] 后台执行并等待
来源：http://hz.tianlin.xyz/gtmugshbdx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtowfcirfn.html

[R36] 并发执行多个任务
来源：http://hz.yuxming.cn/gtlpmzthzw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gtwrpyrvnl.html

[R37] 把输出赋给变量
来源：http://hz.daria6918.cn/gtevajxgab.html

files=$(ls -1)
来源：http://hz.xuetiantiany.cn/gtjlmgrkva.html

[R38] 管道串联
来源：http://hz.aizwys.cn/gtvnjnghsl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.c1oappe.top/gtaujkspvy.html

[R39] 重定向标准输出与错误
来源：http://hz.snrcjt.cn/gtserlbbfd.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtwpdrmbhk.html

[R40] 追加写日志
来源：http://hz.chenjidiqi.icu/gtlpgyzkeg.html

echo "log" >> out.log
来源：http://hz.zhiwuduotai.top/gtsdtavlwo.html

[R41] 丢弃输出
来源：http://hz.nanxinkj.top/gtovovfteu.html

cmd >/dev/null 2>&1
来源：http://hz.jinghuilouyu.cn/gtqfnnwpaf.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gtvjvmbtsw.html

wc -l < a.txt
来源：http://hz.guowangkeji.top/gtzsnnhypa.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtuqxamvor.html

find . -name "*.log" -type f
来源：http://hz.yanxiufei.cn/gthefoivga.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtwxotqqzg.html

find . -mtime -7 -type f
来源：http://hz.cdnleiting.top/gtqcephfpp.html

[R45] 批量删除
来源：http://hz.ywan-chungtsiang.top/gtiumiienh.html

find . -name "*.tmp" -delete
来源：http://hz.sxryk.cn/gtwbwsiwmx.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gtnzqnitlh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtvraiouvn.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gtumndckrf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hammf.cn/gtctdisprf.html

[R48] awk 取指定列
来源：http://hz.nanxuanxn.top/gtqjnbrnrl.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtbhzbeoxt.html

[R49] awk 带条件
来源：http://hz.jinghuilouyu.cn/gtsvvzmysm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jianghu66.top/gtepxqqmbc.html

[R50] awk 求和
来源：http://hz.meibo888.top/gttfbvoxtn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xylfe.cn/gttfjxkbqm.html

[R51] 排序去重取前几
来源：http://hz.gotoacloud.top/gtfabytxos.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ywan-chungtsiang.top/gtuywrkljn.html

[R52] 统计行数
来源：http://hz.jiagoushi.top/gtbgetgara.html

wc -l a.txt
来源：http://hz.redwolf501.top/gtdrayiocq.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtzqtghacc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daxiang520.top/gtsqgbqchn.html

[R54] 比较两个文件
来源：http://hz.xingfuxueyuan.xyz/gtgiubtrvt.html

diff a.txt b.txt
来源：http://hz.gogol.net.cn/gtysfrtyvf.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gteebnhuwo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yanxiufei.cn/gtevteklkt.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtcnsvhnme.html

scp file user@host:/path/
来源：http://hz.ydzc1.top/gthigpaghz.html

[R57] 远程执行命令
来源：http://hz.jiagoushi.top/gtagkobtao.html

ssh user@host 'uptime'
来源：http://hz.fengsongda.top/gtpvbddnml.html

[R58] 下载文件
来源：http://hz.sysykeji.top/gttysgxbpv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtdmvbffgt.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtvaocdrer.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.mhx1999.top/gtdsyepees.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtabcysrpj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yonumen.top/gtmkerwznz.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtiongpcfc.html

df -h;  du -sh *
来源：http://hz.xingfuxueyuan.xyz/gtrkftwzau.html

[R62] 找最占空间的文件
来源：http://hz.ydjk.org.cn/gtutrfrtbe.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258888.top/gtuuctioib.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtgljvwcdz.html

free -h;  ps aux | grep nginx
来源：http://hz.chenjidiqi.icu/gtyoymfxcw.html

[R64] 结束进程
来源：http://hz.gzhubu.top/gtsfrqvrau.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgfzy.top/gtedvzdssv.html

[R65] 查看端口占用
来源：http://hz.tian-w.cn/gtssxlwvev.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nwbrower.top/gtsqosazxu.html

[R66] 定时任务
来源：http://hz.316326.xyz/gtdwyktuqq.html

crontab -e;  crontab -l
来源：http://hz.hfpthk.cn/gtawbfugcs.html

[R67] 生成随机十六进制串
来源：http://hz.xingfuxueyuan.xyz/gtdbvtcanl.html

openssl rand -hex 16
来源：http://hz.shangyingyoupin.top/gteyzkzpio.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtzelkdcvt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtnkkibebj.html

[R69] 生成随机密码
来源：http://hz.ehwqpu.com/gttfepmhoq.html

head -c 16 /dev/urandom | base64
来源：http://hz.tianlin.xyz/gttwittbvv.html

[R70] 时间戳与互转
来源：http://hz.jqgfzy.top/gtxzuxngxc.html

date +%s;  date -d @1700000000
来源：http://hz.daria6918.cn/gtjqrnbgop.html

[R71] 日期格式化
来源：http://hz.gogol.net.cn/gtpamsaazc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhaomingkeji.xyz/gttjcnfcsa.html

[R72] 等待端口就绪
来源：http://hz.chenzaomai.com/gttdtlfssl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nanxinkj.top/gtvbehxvan.html

[R73] 分割大日志
来源：http://hz.9152youxi.cn/gtijduqllz.html

split -l 1000 big.log part_
来源：http://hz.cqqwz.cn/gtrrtkjpmb.html

[R74] 批量重命名
来源：http://hz.yonumen.top/gtmerubkvz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pengpengdd.cyou/gtlrdhwzwl.html

[R75] 导出环境变量
来源：http://hz.nanxinkj.top/gtkeckmwys.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenzaomai.com/gtqiypazdt.html

[R76] 使用临时文件
来源：http://hz.sweek.top/gtnvqeojta.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gtxkwvwwjj.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtkwzpaqzw.html

read -rp "请输入: " ans
来源：http://hz.nanxinkj.top/gticpgdyix.html

[R78] 交互式菜单
来源：http://hz.sysykeji.top/gtxwarihtd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuanzhike.top/gtadslbceg.html

[R79] 解析命令行选项
来源：http://hz.aibaodan.cn/gtimmclszc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtxxytiakj.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtioecdvdh.html

time ./run.sh
来源：http://hz.yangfankeji.com/gtopyfqbmo.html

================================================================================
来源：http://hz.gotoacloud.top/gtxaerewxd.html

S. C / C++ 专题
来源：http://hz.xingfuxueyuan.xyz/gtdotsrfav.html

================================================================================
来源：http://hz.aizwys.cn/gtnvrlclbw.html

[S01] C：Hello World
来源：http://hz.redwolf501.top/gtikdpvzpk.html

#include <stdio.h>
来源：http://hz.shanyushiyangtech.top/gtcnrituss.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yueranfly.top/gtqxgldrdc.html

[S02] C：变量与格式化输出
来源：http://hz.fzhhl.top/gtwpxqzzwa.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangtech.top/gtjpvblrog.html

[S03] C：读入整数
来源：http://hz.svipenyu.cn/gtbquqnpsx.html

int x; scanf("%d", &x);
来源：http://hz.316326.xyz/gtbkaknoht.html

[S04] C：字符串复制
来源：http://hz.nwbrower.top/gtyzxkoqkw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.fzhhl.top/gtnhzyecor.html

[S05] C：字符串长度
来源：http://hz.ydzc1.top/gtkmtxmmdg.html

strlen(s)
来源：http://hz.gzhubu.top/gtxzdijdiz.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtxhloivyw.html

strcmp(a, b) == 0
来源：http://hz.guannengcc.top/gtdxdcwhdi.html

[S07] C：数组遍历求和
来源：http://hz.sxryk.cn/gtjjaeykwy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tanke756.top/gteazvklpv.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigfzy.top/gtxxzbvydp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xylfe.cn/gtbinewqly.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtuwbnqpuu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtqsxfpjld.html

[S10] C：指针与解引用
来源：http://hz.aizwys.cn/gtmgwjevfi.html

int *p = &a;  *p = 5;
来源：http://hz.jinyuanbaomall.cn/gtddugzfjg.html

[S11] C：逐行读文件
来源：http://hz.ehwqpu.com/gtztpiwiwi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.kuanghao11.cn/gtbfsavaff.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.birdmap.top/gtjrzudwim.html

fclose(f);
来源：http://hz.nwbrower.top/gtittfwwxs.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gtcqjedwun.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtutqbbxhf.html

[S13] C：宏定义
来源：http://hz.ehwqpu.com/gtsywxhqjg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtftffvqmk.html

[S14] C：枚举
来源：http://hz.hnqzz.top/gtoqrpytbv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yangfankeji.com/gtgxdtkpam.html

[S15] C：类型转换
来源：http://hz.quarkkingdee.top/gtnztgecgo.html

(double) a / b
来源：http://hz.kuanghao11.cn/gtryebpnzu.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtdbavhbwx.html

x |= (1 << 3);
来源：http://hz.cheryme.top/gtfowvohsc.html

[S17] C：安全拼接字符串
来源：http://hz.zhiwuduotai.top/gtctbouhik.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ppjwa.cn/gteusclxop.html

[S18] C：命令行参数
来源：http://hz.jqgfzy.top/gtqdoveqce.html

int main(int argc, char **argv)
来源：http://hz.daxiang520.top/gtjpmqdpqe.html

[S19] C：快速排序
来源：http://hz.redwolf501.top/gtkbcbqctw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtoeshghre.html

[S20] C：二分查找
来源：http://hz.yvedp.cn/gtmombzdcx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtnexmszao.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gticekaulh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shzxlz.cn/gtqkzfexzd.html

[S22] C：字符串转数字
来源：http://hz.shangyingyoupin.top/gtaahnzvfd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.andypj.xyz/gtuikvqmsg.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gtxbsseihz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.havefunace.top/gtkryabjak.html

[S24] C：获取本地时间
来源：http://hz.yonumen.top/gtojlhxtry.html


<!-- 参考信息 -->