代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hysaishi.cn/gtesdpcryw.html

[Q50] 批量更新
来源：http://hz.jqgufenzy.top/gthizdnjdt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guannengcc.top/gtjxmkglng.html

[Q51] 用子查询更新
来源：http://hz.hysaishi.cn/gtdvxnsjzy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydjk.org.cn/gtxjajfbmy.html

[Q52] 删除指定行
来源：http://hz.havefunace.top/gteqpdhzxo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtxfjjfmnh.html

[Q53] 按条件删除
来源：http://hz.jianghu66.top/gtrqwzszrp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxuanxn.top/gtusbpyuch.html

[Q54] 清空表
来源：http://hz.daxiang520.top/gticrrucgi.html

TRUNCATE TABLE logs;
来源：http://hz.pengpengdd.cyou/gtdtcojlcd.html

[Q55] 排名（并列占位）
来源：http://hz.wangshuangyany.cn/gtuhauyofz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gthrheurch.html

[Q56] 密集排名（并列不占位）
来源：http://hz.bjfxy.top/gtgbelzrcl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258888.top/gtsdeliqpq.html

[Q57] 行号
来源：http://hz.fengsongda.top/gtufileggj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hfpthk.cn/gtynsrrfyx.html

[Q58] 累计求和
来源：http://hz.xylfe.cn/gtmaibjqgo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuxming.cn/gtdyclzxbe.html

[Q59] 分组内累计
来源：http://hz.9152youxi.cn/gtvkgwtrpf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sysykeji.top/gtqdtqveuh.html

[Q60] 取上一行 / 下一行
来源：http://hz.gzhubu.top/gtjicrwynv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtuvaaeaea.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gogol.net.cn/gtdgzmdauk.html

[Q61] 移动平均
来源：http://hz.daria6918.cn/gtiglrthyc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fzhhl.top/gtkqffmqot.html

[Q62] 分组占比
来源：http://hz.zhiwuduotai.top/gtgkzkkhsf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtqgufkhhu.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtoxngjdkh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jyoumei.cn/gttfvcvyvt.html

[Q64] 提交事务
来源：http://hz.xinyue.icu/gtgmtrsfsj.html

COMMIT;
来源：http://hz.ydjk.org.cn/gtjbhjjmnn.html

[Q65] 回滚事务
来源：http://hz.zhoulong.xyz/gtlqijfsio.html

ROLLBACK;
来源：http://hz.zhongyouzk.top/gtgugoglsh.html

[Q66] 行锁查询
来源：http://hz.wangshuangyany.cn/gtmgzdkhnt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sweek.top/gtaxmeavqu.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtdusofxbk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yueranfly.top/gtmmaefmbm.html

[Q68] 保存点
来源：http://hz.tanke756.top/gtnjdyxqji.html

SAVEPOINT sp1;
来源：http://hz.yueranfly.top/gtzdilpcrl.html

ROLLBACK TO sp1;
来源：http://hz.nanxuanxn.top/gtshhmkyze.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtnykkqjya.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhijiandao.cn/gtrbaqntac.html

[Q70] 更新统计信息
来源：http://hz.svipenyu.cn/gtpbapoljh.html

ANALYZE TABLE users;
来源：http://hz.jianghu66.top/gtojocqnwv.html

[Q71] 查看建表语句
来源：http://hz.chenjidiqi.icu/gtvuirzorm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yangfankeji.com/gtvpksigzt.html

[Q72] 查看索引
来源：http://hz.birdmap.top/gtcrwzfryj.html

SHOW INDEX FROM users;
来源：http://hz.pengpengdd.cyou/gtxcyqoaxd.html

[Q73] 查看表状态
来源：http://hz.chenlongwang.top/gtznsejugp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.52xcode.cn/gtakjdeoys.html

[Q74] 强制使用索引
来源：http://hz.jqgufenzy.top/gtswfsrqyi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shangyingyoupin.top/gtazyhdzsu.html

[Q75] 日期格式化
来源：http://hz.pengpengdd.cyou/gtbxpndbwq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtnvyvatwd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gttjfbpffc.html

[Q76] 按天统计
来源：http://hz.xuanzx.com/gtolqcvlfe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cdnleiting.top/gtjpywfbig.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gtncklyvqd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pengpengdd.cyou/gtrxgnfurw.html

[Q78] 当前时间
来源：http://hz.zdqjudy.top/gtfhxnbfqd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.feifeiyinyue.top/gtqektjbky.html

[Q79] 字符串拼接
来源：http://hz.fengsongda.top/gtatspgaei.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.316326.xyz/gtkeihcfnd.html

[Q80] 字符串截取
来源：http://hz.hammf.cn/gtptpvxklq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hysaishi.cn/gteoklfgiz.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtfbzyaggr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgufenzy.top/gtnhhnjafl.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtxjlawtso.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.mhx1999.top/gtdzbtbjoq.html

[Q83] 大小写转换
来源：http://hz.nwbrower.top/gtdgdrrzgv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtqtgxbvmu.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtpsdmnhnw.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtqbvjcpzv.html

[Q85] 数值取整
来源：http://hz.yj20258888.top/gtsqkkifnl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtcwpbbgkb.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gtezjjryqr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hywenlv.cn/gtdcpaecji.html

[Q87] JSON 字段做条件
来源：http://hz.xziqi.cn/gtoyshcvor.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yanxiufei.cn/gtiqneupko.html

[Q88] 行转列（条件聚合）
来源：http://hz.birdmap.top/gtpxhuraas.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258.top/gtkeoapjnh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ybcxt.top/gtjautdoxb.html

[Q89] 判断表是否存在
来源：http://hz.shuidangran.top/gtvkiaiwgk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sufxvd.cn/gtxxtpemmy.html

[Q90] 生成序号列
来源：http://hz.hysaishi.cn/gtkhqrxpsr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gogol.net.cn/gtkyuyrozk.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtohovlxvb.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtsmlnzmug.html

================================================================================
来源：http://hz.cheryme.top/gtnuxhyatl.html

[R01] shebang 与严格模式
来源：http://hz.wangshuangyany.cn/gtwvbmzbyz.html

#!/usr/bin/env bash
来源：http://hz.smart0.xyz/gtabgxusmd.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtcvignafu.html

[R02] 变量赋值与使用
来源：http://hz.smart0.xyz/gtythfaily.html

name="Tom"; echo "$name"
来源：http://hz.feifeiyinyue.top/gtvdqbtkzg.html

[R03] 只读变量
来源：http://hz.shuidangran.top/gtovlxvtvd.html

readonly PI=3.14
来源：http://hz.daxiang520.top/gtzpqcchzc.html

[R04] 位置参数
来源：http://hz.birdmap.top/gtskshnscm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.quarkkingdee.top/gtvkokldup.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gtpodayfrt.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtjcpzpeqe.html

[R06] 判断命令是否存在
来源：http://hz.zhaomingkeji.xyz/gtvsfwelcc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtvejuuoam.html

[R07] if 判断文件
来源：http://hz.jinqigfzy.top/gtojuuzsdd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gzhubu.top/gttjfwlakt.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtsptudfqr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj202588.top/gtvynrgbop.html

[R09] 字符串比较
来源：http://hz.hammf.cn/gtkkgzhjed.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhiwuduotai.top/gtgpayhnvw.html

[R10] 正则匹配
来源：http://hz.smart0.xyz/gtprqtbduo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.haohaochexian.top/gtpqqhmejs.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtbeywofsu.html

case "$1" in
来源：http://hz.xuanzx.com/gtmvlmjhns.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gttpulptgh.html

stop)  echo "停止" ;;
来源：http://hz.iojbl.cn/gtrtsdqety.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gttywauufq.html

esac
来源：http://hz.sufxvd.cn/gtosortxph.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtrzqlwonh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pycfn.com/gtucruclad.html

[R13] for 计数循环
来源：http://hz.fzhhl.top/gtzibocibz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tianlin.xyz/gtcbczviee.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gthhshaqll.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgfzy.top/gtgswfbjqs.html

[R15] while 逐行读文件
来源：http://hz.yongpay.top/gtuyvyahvz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.havefunace.top/gtojjzwkrq.html

[R16] until 等待条件
来源：http://hz.yj20258888.top/gthcbwqjgk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cdnleiting.top/gtllubmkos.html

[R17] 数组定义与取值
来源：http://hz.jinyuanbaomall.cn/gtpooeizcm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zdqjudy.top/gtjeseupni.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gtkxbljmrf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cqqwz.cn/gtkrhtehfx.html

[R19] 数组长度
来源：http://hz.gzhubu.top/gtqcgkeueo.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtpedckvsm.html

[R20] 关联数组（字典）
来源：http://hz.snrcjt.cn/gtkteyoyow.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtvyooukro.html

[R21] 字符串长度
来源：http://hz.zhixingplan.top/gtvrjiugvw.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtbskmekzy.html

[R22] 截取子串
来源：http://hz.zhoulong.xyz/gtrjjupzjz.html

echo "${s:0:5}"
来源：http://hz.yj202588.top/gtfcuaowih.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtdpkcraks.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gzhubu.top/gtmdfkmbnk.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gthrycirub.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tian-w.cn/gtglcapioh.html

[R25] 去后缀 / 去前缀
来源：http://hz.gogol.net.cn/gtphzllxtr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ivvv.top/gtnqfataqi.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtqiqiisiy.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gtkosunuzc.html

[R27] 算术展开
来源：http://hz.guannengcc.top/gtshxkhwcv.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtmgymdvdw.html

[R28] 浮点运算
来源：http://hz.0kj1m.cn/gtzdcjwafl.html

echo "scale=2; 10/3" | bc
来源：http://hz.dianchejie.cn/gtbymxzqfi.html

[R29] 定义函数
来源：http://hz.hnxiangtu.top/gtxnwjqbil.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenlongwang.top/gtlzqgmzgd.html

[R30] 函数返回状态码
来源：http://hz.c1oappe.top/gtgdgwdows.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtsnbrsvgl.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gtcvwfdmhi.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnxiangtu.top/gtesxmanuu.html

[R32] 参数个数校验
来源：http://hz.cashguo.top/gtvnlqdeku.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tanke756.top/gtwqoxpbio.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtvjnwufaj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.quarkkingdee.top/gtejivtfhz.html

[R34] 退出时清理
来源：http://hz.guannengcc.top/gtuoorhbif.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtcippgrxm.html

[R35] 后台执行并等待
来源：http://hz.yueranfly.top/gtqzzsrebq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhongyouzk.top/gtkfxhsjaw.html

[R36] 并发执行多个任务
来源：http://hz.cdnleiting.top/gtqjdckinu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.316326.xyz/gtrkzcbhtm.html

[R37] 把输出赋给变量
来源：http://hz.zhongyouzk.top/gtqdcixfeu.html

files=$(ls -1)
来源：http://hz.jianghu66.top/gtqjvpppyo.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtutgfcsjp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xylfe.cn/gtzuirozxg.html

[R39] 重定向标准输出与错误
来源：http://hz.xuetiantiany.cn/gtcvcolqpr.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtrknpocfb.html

[R40] 追加写日志
来源：http://hz.zhaomingkeji.xyz/gtqhfclmqq.html

echo "log" >> out.log
来源：http://hz.sysykeji.top/gtiwwxniik.html

[R41] 丢弃输出
来源：http://hz.aizwys.cn/gtggsllpvm.html

cmd >/dev/null 2>&1
来源：http://hz.nanxuanxn.top/gttznshkhf.html

[R42] 输入重定向
来源：http://hz.hywenlv.cn/gtdsnwlcyb.html

wc -l < a.txt
来源：http://hz.zhijiandao.cn/gtebcharrl.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtljbjfddg.html

find . -name "*.log" -type f
来源：http://hz.jlsjyb.cn/gtpdgavydx.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gtmdhgqpjd.html

find . -mtime -7 -type f
来源：http://hz.zhijiandao.cn/gtftwukzgm.html

[R45] 批量删除
来源：http://hz.haohaochexian.top/gtntajwtix.html

find . -name "*.tmp" -delete
来源：http://hz.dashuyun.cn/gtorrljafs.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gtaveuceyu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.redwolf501.top/gtbzrkwcvo.html

[R47] sed 单行替换
来源：http://hz.gotoacloud.top/gttzqxhoyu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhijiandao.cn/gtfttnbknm.html

[R48] awk 取指定列
来源：http://hz.kuanghao11.cn/gtslexxmyi.html

awk '{print $1, $3}' a.txt
来源：http://hz.cashguo.top/gthektrwpr.html

[R49] awk 带条件
来源：http://hz.ybcxt.top/gtaetqjcka.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtluhvhugd.html

[R50] awk 求和
来源：http://hz.aibaodan.cn/gtixqdioxo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gtvhwhdgjz.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gtavgeckvw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xziqi.cn/gttshfauph.html

[R52] 统计行数
来源：http://hz.snrcjt.cn/gtesuercab.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gthcaacxsc.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtafwqsbot.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jqgufenzy.top/gttbuokkec.html

[R54] 比较两个文件
来源：http://hz.havefunace.top/gtvlscmxue.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gtcsfiuptw.html

[R55] 压缩与解压
来源：http://hz.guannengcc.top/gtxkmxylpj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.andypj.xyz/gtnkikvgxk.html

[R56] 远程拷贝
来源：http://hz.hongshengwenyu.top/gtxaptlyrm.html

scp file user@host:/path/
来源：http://hz.jinyuanbaomall.cn/gtrhubfcol.html

[R57] 远程执行命令
来源：http://hz.jqgufenzy.top/gtfvouzqei.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gtcxbafwxm.html

[R58] 下载文件
来源：http://hz.ppjwa.cn/gtbwajrayb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jiagoushi.top/gtwinqygoi.html

[R59] 发 POST JSON
来源：http://hz.yanxiufei.cn/gthjkymxzg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gtdkaaqqov.html

[R60] 只看 HTTP 状态码
来源：http://hz.dashuyun.cn/gtxkjhmynb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgfzy.top/gtlendyanv.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtyaoakslq.html

df -h;  du -sh *
来源：http://hz.yuxming.cn/gtumbspcnm.html

[R62] 找最占空间的文件
来源：http://hz.kuanghao11.cn/gtzcujqmxh.html

du -ah . | sort -rh | head -10
来源：http://hz.shzxlz.cn/gtckugiamy.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtqrynposb.html

free -h;  ps aux | grep nginx
来源：http://hz.jianghu66.top/gtnhjpaqir.html

[R64] 结束进程
来源：http://hz.yuanzhike.top/gtjmucuefb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.dianchejie.cn/gtehdmvdqp.html

[R65] 查看端口占用
来源：http://hz.guowangkeji.top/gtlfpexaux.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhoulong.xyz/gtbgpqhsnq.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtdouogmpv.html

crontab -e;  crontab -l
来源：http://hz.aizwys.cn/gtcjqksthz.html

[R67] 生成随机十六进制串
来源：http://hz.hysaishi.cn/gtttgofvcy.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gteqcrqzoa.html

[R68] 计算文件校验值
来源：http://hz.jianghu66.top/gtsmnjuosj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtzvazwebk.html

[R69] 生成随机密码
来源：http://hz.yj202588.top/gtpzpunego.html

head -c 16 /dev/urandom | base64
来源：http://hz.meibo888.top/gtyzjkdrwq.html

[R70] 时间戳与互转
来源：http://hz.yangfankeji.com/gtpxuexqxw.html

date +%s;  date -d @1700000000
来源：http://hz.hywenlv.cn/gtjbxgsmlu.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtadbkckws.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.meibo888.top/gtgzwojehm.html

[R72] 等待端口就绪
来源：http://hz.chenzaomai.com/gtsukflqub.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gzhubu.top/gtlacboxbr.html

[R73] 分割大日志
来源：http://hz.aibaodan.cn/gttnacvwdt.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangkeji.top/gtcuscvgws.html

[R74] 批量重命名
来源：http://hz.andypj.xyz/gtdvwjodle.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gotoacloud.top/gtcueanord.html

[R75] 导出环境变量
来源：http://hz.fzhhl.top/gtzckwonrp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.c1oappe.top/gtzoyekldt.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangtech.top/gtgmwqlmlr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtylgzwque.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtexlmewzf.html

read -rp "请输入: " ans
来源：http://hz.jinghuilouyu.cn/gtgiaocjqo.html

[R78] 交互式菜单
来源：http://hz.shangyingyoupin.top/gtrowfancn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258.top/gtjdipmtrb.html

[R79] 解析命令行选项
来源：http://hz.vqdsnc.cn/gtmhdvcyeh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daxiang520.top/gtadetdaru.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtamrqeynl.html

time ./run.sh
来源：http://hz.tanke756.top/gtcovluaol.html

================================================================================
来源：http://hz.zhongyouzk.top/gtudbrlizh.html

S. C / C++ 专题
来源：http://hz.sweek.top/gtducerncv.html

================================================================================
来源：http://hz.birdmap.top/gtpokdpvfb.html

[S01] C：Hello World
来源：http://hz.52xcode.cn/gtuzorrnvz.html

#include <stdio.h>
来源：http://hz.jianghu66.top/gtfadpmhec.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydzc1.top/gtgiafyhwv.html

[S02] C：变量与格式化输出
来源：http://hz.mhx1999.top/gtldcjbflc.html

int a = 10; printf("%d\n", a);
来源：http://hz.ppjwa.cn/gtbuiyqgfj.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gtctupudbj.html

int x; scanf("%d", &x);
来源：http://hz.aizwys.cn/gtbadiutwy.html

[S04] C：字符串复制
来源：http://hz.havefunace.top/gtzjimpyzf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ywan-chungtsiang.top/gtthgrjmcy.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtrokcjsgr.html

strlen(s)
来源：http://hz.cdnleiting.top/gtpwpqhycm.html

[S06] C：字符串比较
来源：http://hz.cdnleiting.top/gtafimdxdi.html

strcmp(a, b) == 0
来源：http://hz.xinyue.icu/gtrzvqghyk.html

[S07] C：数组遍历求和
来源：http://hz.havefunace.top/gtiqqzqqik.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj20258888.top/gtsxuytjlw.html

[S08] C：动态内存分配与释放
来源：http://hz.daxiang520.top/gtevzctpcz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxinkj.top/gtfvlnvomt.html

[S09] C：结构体定义与初始化
来源：http://hz.cucudq.cn/gtubbjbqof.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhoulong.xyz/gtqhnkxtau.html

[S10] C：指针与解引用
来源：http://hz.zhijiandao.cn/gtamgurarw.html

int *p = &a;  *p = 5;
来源：http://hz.jinyuanbaomall.cn/gtpnurdznz.html

[S11] C：逐行读文件
来源：http://hz.fzhhl.top/gtlyktnfui.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ywan-chungtsiang.top/gtbpiqtlub.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.316326.xyz/gtybrkmbvb.html

fclose(f);
来源：http://hz.iojbl.cn/gtynjjsxqu.html

[S12] C：写文件
来源：http://hz.pycfn.com/gtctvueyhz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ybcxt.top/gtxgtboaxs.html

[S13] C：宏定义
来源：http://hz.quarkkingdee.top/gteafamfbe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ywan-chungtsiang.top/gttjzldogn.html

[S14] C：枚举
来源：http://hz.aibaodan.cn/gtjricflsy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gtfyhpmlru.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtejapvgwu.html

(double) a / b
来源：http://hz.nanxinkj.top/gtwxijbxfr.html

[S16] C：位操作置位
来源：http://hz.jinghuilouyu.cn/gtzgktiunu.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gtljfgxzai.html

[S17] C：安全拼接字符串
来源：http://hz.yangfankeji.com/gthclmvkhk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.quarkkingdee.top/gtlwadgkmk.html

[S18] C：命令行参数
来源：http://hz.316326.xyz/gtafbjqhqo.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gthwtucldt.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gtjbmxrqfn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtokjoblzs.html

[S20] C：二分查找
来源：http://hz.jianghu66.top/gtzmwkqbfd.html


<!-- 参考信息 -->