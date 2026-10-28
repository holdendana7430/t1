代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ppjwa.cn/gtmmazldax.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tanke756.top/gttngxjhhb.html

[Q39] 自连接（查上下级）
来源：http://hz.pycfn.com/gtnkrqeofk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydjk.org.cn/gtlcyacvdz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhengqikj.top/gtlwmexdzj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sufxvd.cn/gtqbtkilsq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.haohaochexian.top/gtblpkjxsf.html

[Q41] 多表连接
来源：http://hz.gzhubu.top/gtmzwcargu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtstxgysvt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ehwqpu.com/gtdvipjtwt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yueranfly.top/gtkbkciirv.html

[Q42] 连接条件附加过滤
来源：http://hz.sysykeji.top/gtcpsmppqv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.redwolf501.top/gtohuetfok.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jlsjyb.cn/gtosjitdym.html

[Q43] 标量子查询
来源：http://hz.shzxlz.cn/gtqrpvtfic.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuanzx.com/gtewwuuavi.html

[Q44] IN 子查询
来源：http://hz.hysaishi.cn/gtgtrodgfs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.svipenyu.cn/gtfvznzcov.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigufen.top/gtmiximmdz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtyrhflcms.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shzxlz.cn/gtpcassvop.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtwnmzlihi.html

[Q47] 与平均值比较
来源：http://hz.smart0.xyz/gtouggdehw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.quarkkingdee.top/gtiwurloeg.html

[Q48] CTE 公用表表达式
来源：http://hz.kuanghao11.cn/gtxfkptrme.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tian-w.cn/gtekbvzops.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jianghu66.top/gtnztqpqsv.html

[Q49] 更新单行
来源：http://hz.pycfn.com/gtuurqnlgy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.bjfxy.top/gtyervjczd.html

[Q50] 批量更新
来源：http://hz.mhx1999.top/gtltdeldoh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.0kj1m.cn/gtqpzhlpil.html

[Q51] 用子查询更新
来源：http://hz.wangdashe.top/gtpmstfxrn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydjk.org.cn/gtfbtckovf.html

[Q52] 删除指定行
来源：http://hz.hongshengwenyu.top/gtykkvgzgs.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gtmgoptazb.html

[Q53] 按条件删除
来源：http://hz.tanke756.top/gtxgfzxzke.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yonumen.top/gtzjhgsnfh.html

[Q54] 清空表
来源：http://hz.zhiwuduotai.top/gtmdymlflg.html

TRUNCATE TABLE logs;
来源：http://hz.hywenlv.cn/gtrmhhjjpi.html

[Q55] 排名（并列占位）
来源：http://hz.gzhubu.top/gtpprqffme.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.fzhhl.top/gtgolonkcq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangtech.top/gtruvnwyxg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtldxuadzb.html

[Q57] 行号
来源：http://hz.cucudq.cn/gtceaawuel.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.feifeiyinyue.top/gtderzbhem.html

[Q58] 累计求和
来源：http://hz.jqgufenzy.top/gteixvsaxi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuxming.cn/gtdalvgwnz.html

[Q59] 分组内累计
来源：http://hz.cqqwz.cn/gtyepjojlr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dashuyun.cn/gtoorkybnb.html

[Q60] 取上一行 / 下一行
来源：http://hz.svipenyu.cn/gtlrjrhnhv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xziqi.cn/gtcmjdzxho.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenjidiqi.icu/gtvayhvxdu.html

[Q61] 移动平均
来源：http://hz.ivvv.top/gthykqcjac.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yangfankeji.com/gtjtaldcni.html

[Q62] 分组占比
来源：http://hz.zhijiandao.cn/gtkgjyqkba.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtunlnamhc.html

[Q63] 开启事务
来源：http://hz.ydzc1.top/gtpbcicahs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gzhubu.top/gtqixzrjcm.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gtcnwccyom.html

COMMIT;
来源：http://hz.dianchejie.cn/gtutspvdcp.html

[Q65] 回滚事务
来源：http://hz.zhiwuduotai.top/gtounjmqgq.html

ROLLBACK;
来源：http://hz.xingfuxueyuan.xyz/gtultrmzoq.html

[Q66] 行锁查询
来源：http://hz.cucudq.cn/gtxrnwkyfg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhixingplan.top/gtenejglaa.html

[Q67] 设置隔离级别
来源：http://hz.wangdashe.top/gtrxlolcyb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenlongwang.top/gtnzwzgtql.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtuksighfh.html

SAVEPOINT sp1;
来源：http://hz.sweek.top/gtywtdoozs.html

ROLLBACK TO sp1;
来源：http://hz.dianchejie.cn/gtwkuqibmx.html

[Q69] 查看执行计划
来源：http://hz.jiagoushi.top/gtonfhivoz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtnkblihze.html

[Q70] 更新统计信息
来源：http://hz.daria6918.cn/gtzlixphcj.html

ANALYZE TABLE users;
来源：http://hz.yuxming.cn/gtjmuufirk.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangtech.top/gtlolhbcsy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xziqi.cn/gtvkvsyleq.html

[Q72] 查看索引
来源：http://hz.ehwqpu.com/gtoouefkaj.html

SHOW INDEX FROM users;
来源：http://hz.nanxuanxn.top/gtpnhyydso.html

[Q73] 查看表状态
来源：http://hz.cheryme.top/gtolipdwbr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xziqi.cn/gtzoltdcfp.html

[Q74] 强制使用索引
来源：http://hz.kuanghao11.cn/gtrwmdycca.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tian-w.cn/gtuiiasuko.html

[Q75] 日期格式化
来源：http://hz.aizwys.cn/gtmgtlgfdr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhijiandao.cn/gtuaadbdrp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.fzhhl.top/gtktqxgctt.html

[Q76] 按天统计
来源：http://hz.xylfe.cn/gtejxkraxf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhongyouzk.top/gthdzuuseo.html

[Q77] 时间加减
来源：http://hz.ydjk.org.cn/gthonjnxsl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yangfankeji.com/gtlshbmqtu.html

[Q78] 当前时间
来源：http://hz.gzhubu.top/gtfkvlaijd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.0kj1m.cn/gtrvmekhjm.html

[Q79] 字符串拼接
来源：http://hz.zdqjudy.top/gtcpvfwcwx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhiwuduotai.top/gtytfhqdfa.html

[Q80] 字符串截取
来源：http://hz.yongpay.top/gtovyeyhxd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yueranfly.top/gtwmqnwbuj.html

[Q81] 字符串替换
来源：http://hz.feifeiyinyue.top/gtgbysuzhw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuetiantiany.cn/gtwsbcyhpl.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtqsiqrntf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.haohaochexian.top/gtrqtpopnf.html

[Q83] 大小写转换
来源：http://hz.dianchejie.cn/gtiujdqrwb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gotoacloud.top/gtbtotiiwj.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gtjngpmcid.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhoulong.xyz/gthfbecjcj.html

[Q85] 数值取整
来源：http://hz.xingfuxueyuan.xyz/gtoaizezvf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gtmjbihvtq.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtmvsbdpfe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yonumen.top/gtszpjygfg.html

[Q87] JSON 字段做条件
来源：http://hz.shuidangran.top/gtykohkhsn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zycfv.cn/gtkeisfayw.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhengqikj.top/gthtpfquac.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hywenlv.cn/gtjvzahfrc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtupwiyjkg.html

[Q89] 判断表是否存在
来源：http://hz.tianlin.xyz/gttpnnfshs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtjvkpbmbf.html

[Q90] 生成序号列
来源：http://hz.pengpengdd.cyou/gtdavrueya.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhoulong.xyz/gtvmwltfnf.html

================================================================================
来源：http://hz.kuanghao11.cn/gtoqhwbjou.html

R. Bash 专题
来源：http://hz.xziqi.cn/gtxugwffan.html

================================================================================
来源：http://hz.gotoacloud.top/gtpqforsqj.html

[R01] shebang 与严格模式
来源：http://hz.shuidangran.top/gtgtkuhxut.html

#!/usr/bin/env bash
来源：http://hz.hfpthk.cn/gtqxyvcxju.html

set -euo pipefail
来源：http://hz.xingfuxueyuan.xyz/gtwqhsfmsw.html

[R02] 变量赋值与使用
来源：http://hz.vqdsnc.cn/gtnqpdvlzi.html

name="Tom"; echo "$name"
来源：http://hz.chenzaomai.com/gtlloqwdqk.html

[R03] 只读变量
来源：http://hz.xinyue.icu/gtectvhwtr.html

readonly PI=3.14
来源：http://hz.birdmap.top/gtiadrqynr.html

[R04] 位置参数
来源：http://hz.fzhhl.top/gtexnpckzv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yueranfly.top/gtqstnnlls.html

[R05] 参数默认值
来源：http://hz.hysaishi.cn/gttynvxyxi.html

name="${1:-default}"
来源：http://hz.chenzaomai.com/gtmxqdliqw.html

[R06] 判断命令是否存在
来源：http://hz.snrcjt.cn/gtvlnslqnx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtnupdvcsr.html

[R07] if 判断文件
来源：http://hz.jianghu66.top/gtfoqedhem.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xuetiantiany.cn/gtwrturrzc.html

[R08] 数值比较
来源：http://hz.iojbl.cn/gtmzpftcwm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zdqjudy.top/gtduilmsrv.html

[R09] 字符串比较
来源：http://hz.sweek.top/gtkwzkhxim.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ivvv.top/gtvkzftvgz.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtclsyhucj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.quarkkingdee.top/gtmpelibzk.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtyuckstif.html

case "$1" in
来源：http://hz.yj20258888.top/gtwiilmxit.html

start) echo "启动" ;;
来源：http://hz.ywan-chungtsiang.top/gtufqqxhbd.html

stop)  echo "停止" ;;
来源：http://hz.hysaishi.cn/gtnfnrlumu.html

*)     echo "未知命令" ;;
来源：http://hz.zhiwuduotai.top/gtglozxddq.html

esac
来源：http://hz.xuetiantiany.cn/gtnwdmfjbt.html

[R12] for 遍历文件
来源：http://hz.nanxuanxn.top/gtvypvlnuq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tanke756.top/gtuaxbnjal.html

[R13] for 计数循环
来源：http://hz.chenlongwang.top/gttayztzat.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj202588.top/gtanqtsbux.html

[R14] C 风格 for
来源：http://hz.ybcxt.top/gtvzknfwea.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtjaxbnzox.html

[R15] while 逐行读文件
来源：http://hz.zhixingplan.top/gtokzotgzx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.mhx1999.top/gthiphuxgw.html

[R16] until 等待条件
来源：http://hz.dianchejie.cn/gtlptblgwh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj202588.top/gtjhbbvxsv.html

[R17] 数组定义与取值
来源：http://hz.yongpay.top/gtjrklpssn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtptkzqdef.html

[R18] 遍历数组
来源：http://hz.xuetiantiany.cn/gtfrouivlh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuanzx.com/gtwcstcobb.html

[R19] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtnbiirvvx.html

echo "${#arr[@]}"
来源：http://hz.xinyue.icu/gtogcxwdnm.html

[R20] 关联数组（字典）
来源：http://hz.jinyuanbaomall.cn/gtnjsilqir.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhixingplan.top/gtjrrsakul.html

[R21] 字符串长度
来源：http://hz.cashguo.top/gtfisdjynj.html

echo "${#s}"
来源：http://hz.smart0.xyz/gtbonswrrv.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtigwwwnve.html

echo "${s:0:5}"
来源：http://hz.ydjk.org.cn/gtqjaslczu.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gthbczcuom.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtlmvjjmck.html

[R24] 大小写转换
来源：http://hz.ehwqpu.com/gtarblvujq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangtech.top/gtnwweozmx.html

[R25] 去后缀 / 去前缀
来源：http://hz.shzxlz.cn/gtcysaaedj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shangyingyoupin.top/gtlumeyuwt.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtvaryphvm.html

now=$(date +%F); echo "$now"
来源：http://hz.ppjwa.cn/gtpmhargxw.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gtmavypwos.html

echo $((1 + 2 * 3))
来源：http://hz.pengpengdd.cyou/gtkawtsbci.html

[R28] 浮点运算
来源：http://hz.hammf.cn/gtjqhzqcdg.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtwcatptrj.html

[R29] 定义函数
来源：http://hz.andypj.xyz/gtinbcyumf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hongshengwenyu.top/gtkfmpistm.html

[R30] 函数返回状态码
来源：http://hz.fzhhl.top/gtvkknowzv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtapyvhhbn.html

[R31] 局部变量
来源：http://hz.yuxming.cn/gtlinfvxsx.html

f() { local x=1; echo "$x"; }
来源：http://hz.ppjwa.cn/gtaecscmhv.html

[R32] 参数个数校验
来源：http://hz.52xcode.cn/gtrexmgtea.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtzwsnsiwp.html

[R33] 捕获错误并提示行号
来源：http://hz.tanke756.top/gtvaolrtit.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.haohaochexian.top/gtchjnscer.html

[R34] 退出时清理
来源：http://hz.xingfuxueyuan.xyz/gtkxrhdmyj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtyeiitvac.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtexiougdq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigfzy.top/gtcwubmjmr.html

[R36] 并发执行多个任务
来源：http://hz.sufxvd.cn/gtnuloixox.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yvedp.cn/gtadcgfvvn.html

[R37] 把输出赋给变量
来源：http://hz.ybcxt.top/gtfhypzooi.html

files=$(ls -1)
来源：http://hz.wangshuangyany.cn/gtpbiqkgrc.html

[R38] 管道串联
来源：http://hz.zhiwuduotai.top/gtssshzggf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dashuyun.cn/gtdoxlduhm.html

[R39] 重定向标准输出与错误
来源：http://hz.sufxvd.cn/gtfkivjbel.html

cmd > out.log 2>&1
来源：http://hz.zhixingplan.top/gtphxvfoqy.html

[R40] 追加写日志
来源：http://hz.aibaodan.cn/gtroyvavvt.html

echo "log" >> out.log
来源：http://hz.tianlin.xyz/gthekupgod.html

[R41] 丢弃输出
来源：http://hz.yueranfly.top/gtytgfqgqx.html

cmd >/dev/null 2>&1
来源：http://hz.gotoacloud.top/gtehsnqefu.html

[R42] 输入重定向
来源：http://hz.c1oappe.top/gtbxhvxqzb.html

wc -l < a.txt
来源：http://hz.gzhubu.top/gtktgovrxe.html

[R43] 按名字查找文件
来源：http://hz.ydjk.org.cn/gtjryzqxly.html

find . -name "*.log" -type f
来源：http://hz.guannengcc.top/gtmzzgzbox.html

[R44] 按修改时间查找
来源：http://hz.sxryk.cn/gtelgouavn.html

find . -mtime -7 -type f
来源：http://hz.sweek.top/gtrmnmotrg.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtewjwmrgs.html

find . -name "*.tmp" -delete
来源：http://hz.yvedp.cn/gtfnorhpab.html

[R46] 递归替换文件内容
来源：http://hz.sysykeji.top/gtgjulmprm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258.top/gthnwkjyyz.html

[R47] sed 单行替换
来源：http://hz.ydzc1.top/gtpuvlhhmr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gtoxtkghbl.html

[R48] awk 取指定列
来源：http://hz.c1oappe.top/gtdkpuurle.html

awk '{print $1, $3}' a.txt
来源：http://hz.hfpthk.cn/gtjubljwlp.html

[R49] awk 带条件
来源：http://hz.gzhubu.top/gtqehfygko.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.bjfxy.top/gtiymkkqpf.html

[R50] awk 求和
来源：http://hz.daxiang520.top/gtekuxucln.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtizpvfmwt.html

[R51] 排序去重取前几
来源：http://hz.fzhhl.top/gtdkzothgo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenlongwang.top/gtuyeqoqqf.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtafaeocpe.html

wc -l a.txt
来源：http://hz.dianchejie.cn/gtsqoeuojr.html

[R53] 查看文件头与实时尾
来源：http://hz.daria6918.cn/gtmvafltjl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtsnyrahkw.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtihxykixe.html

diff a.txt b.txt
来源：http://hz.zycfv.cn/gtysqhxjxq.html

[R55] 压缩与解压
来源：http://hz.yonumen.top/gtjyrqejpb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtlsdncvzh.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gttnmjrqhf.html

scp file user@host:/path/
来源：http://hz.zhiwuduotai.top/gttqofyhor.html

[R57] 远程执行命令
来源：http://hz.guowangkeji.top/gtitmjakor.html

ssh user@host 'uptime'
来源：http://hz.ivvv.top/gtkdybxuwg.html

[R58] 下载文件
来源：http://hz.hnqzz.top/gtkfdxfjep.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangtech.top/gtoppruncb.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtboiqwvov.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.c1oappe.top/gtqpjgzflc.html

[R60] 只看 HTTP 状态码
来源：http://hz.ppjwa.cn/gtybhxxsgc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yuanzhike.top/gtgilpvzdc.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtsgcgqwqy.html

df -h;  du -sh *
来源：http://hz.wangshuangyany.cn/gtxsfoewjy.html

[R62] 找最占空间的文件
来源：http://hz.jinqigufen.top/gtkyomxnnk.html

du -ah . | sort -rh | head -10
来源：http://hz.vqdsnc.cn/gtdzuasycv.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtibzvxrnq.html

free -h;  ps aux | grep nginx
来源：http://hz.snrcjt.cn/gtaaoqpqzb.html

[R64] 结束进程
来源：http://hz.andypj.xyz/gthvpffsve.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtlsztmzbi.html

[R65] 查看端口占用
来源：http://hz.yuanzhike.top/gtxzqrtmih.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yangfankeji.com/gtcgaamwbs.html

[R66] 定时任务
来源：http://hz.shangyingyoupin.top/gtbkrifuaz.html

crontab -e;  crontab -l
来源：http://hz.tian-w.cn/gtdkhmzqlv.html

[R67] 生成随机十六进制串
来源：http://hz.jqgfzy.top/gtkvktkjua.html

openssl rand -hex 16
来源：http://hz.jiagoushi.top/gtbihhpliq.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtspxzyihn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgufenzy.top/gtvxkwblko.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangtech.top/gtsoisamin.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtvqmrcqhg.html

[R70] 时间戳与互转
来源：http://hz.ywan-chungtsiang.top/gtmktzelsy.html

date +%s;  date -d @1700000000
来源：http://hz.birdmap.top/gtiizbgmkr.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtvnxmgtcn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zdqjudy.top/gtrzacjdxp.html

[R72] 等待端口就绪
来源：http://hz.dashuyun.cn/gtbybegwsh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xylfe.cn/gtdkbghskb.html

[R73] 分割大日志
来源：http://hz.hywenlv.cn/gtjdcovndb.html

split -l 1000 big.log part_
来源：http://hz.ppjwa.cn/gtpcdoofrh.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtmfudhicq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangkeji.top/gtddorvupa.html

[R75] 导出环境变量
来源：http://hz.yonumen.top/gtlxkgaiyo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigfzy.top/gtipstshhj.html

[R76] 使用临时文件
来源：http://hz.fzhhl.top/gtqxrpziwy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydzc1.top/gteecqture.html

[R77] 读取用户输入
来源：http://hz.nanxuanxn.top/gtroqfbiop.html

read -rp "请输入: " ans
来源：http://hz.xylfe.cn/gtqxpprfce.html

[R78] 交互式菜单
来源：http://hz.svipenyu.cn/gtkcrpfljn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hfpthk.cn/gtigfjtamw.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtubtpfpxg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhixingplan.top/gtxllijdov.html

[R80] 查看脚本执行耗时
来源：http://hz.gotoacloud.top/gtywtfxroa.html

time ./run.sh
来源：http://hz.cdnleiting.top/gtaqpovqjc.html

================================================================================
来源：http://hz.gzhubu.top/gtihrjbeis.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtxlailwlc.html

================================================================================
来源：http://hz.gogol.net.cn/gtcvdmvfxs.html

[S01] C：Hello World
来源：http://hz.feifeiyinyue.top/gtybwhqpqp.html

#include <stdio.h>
来源：http://hz.pycfn.com/gtekctplvu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aizwys.cn/gtwmmgjouw.html

[S02] C：变量与格式化输出
来源：http://hz.xuetiantiany.cn/gtblxrwtns.html

int a = 10; printf("%d\n", a);
来源：http://hz.quarkkingdee.top/gteufqdsub.html

[S03] C：读入整数
来源：http://hz.hysaishi.cn/gtvdmluuuv.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gtsbdkpohp.html

[S04] C：字符串复制
来源：http://hz.zhaomingkeji.xyz/gtkcbqyttf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shzxlz.cn/gtusdsnnyh.html

[S05] C：字符串长度
来源：http://hz.jinyuanbaomall.cn/gtzfaomist.html

strlen(s)
来源：http://hz.smart0.xyz/gtnlsmgizb.html

[S06] C：字符串比较
来源：http://hz.chenlongwang.top/gtdnvbfrsn.html

strcmp(a, b) == 0
来源：http://hz.aizwys.cn/gtcenqzffs.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtgrskaagq.html


<!-- 参考信息 -->