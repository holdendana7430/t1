代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xylfe.cn/gthqxorwew.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yonumen.top/gtrjantbei.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sxryk.cn/gtvfhlnkuz.html

[Q41] 多表连接
来源：http://hz.shzxlz.cn/gtoxjqxafj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhongyouzk.top/gtybnbezoo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.feifeiyinyue.top/gtehzwymed.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.svipenyu.cn/gtarampsmb.html

[Q42] 连接条件附加过滤
来源：http://hz.xingfuxueyuan.xyz/gtvnmohkgx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gzhubu.top/gtkqeqgwgv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.iojbl.cn/gtuxywfhtw.html

[Q43] 标量子查询
来源：http://hz.chenjidiqi.icu/gtttkxewco.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hysaishi.cn/gtjnjhlrco.html

[Q44] IN 子查询
来源：http://hz.wangshuangyany.cn/gtgxbjmrom.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxuanxn.top/gtxtzprvag.html

[Q45] EXISTS 判断存在
来源：http://hz.yonumen.top/gtbelhndpg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gthylwtxwc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuxming.cn/gtegcwxklt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gttkgqnjbf.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gthznxxxhz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gtwqsvqcbp.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtnwiiqczx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jlsjyb.cn/gtgioopwuw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtgnedfqnc.html

[Q49] 更新单行
来源：http://hz.gaohongyu789.top/gtylguawhk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pycfn.com/gtmfyhlymj.html

[Q50] 批量更新
来源：http://hz.xingfuxueyuan.xyz/gtcgmmihmg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.iojbl.cn/gtwtigjyua.html

[Q51] 用子查询更新
来源：http://hz.cheryme.top/gtfeqcfvzn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sysykeji.top/gttivnbodw.html

[Q52] 删除指定行
来源：http://hz.jiagoushi.top/gtdplqcwtr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtfhmrmvkl.html

[Q53] 按条件删除
来源：http://hz.jinqigufen.top/gtiqfajuao.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hongshengwenyu.top/gtoyjzfgjb.html

[Q54] 清空表
来源：http://hz.ehwqpu.com/gteomgtjft.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtsynrcjwq.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangkeji.top/gtqiztaqzu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hywenlv.cn/gtvlhqezki.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gteanqnngl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgfzy.top/gtvkjxnpws.html

[Q57] 行号
来源：http://hz.gogol.net.cn/gtzeitgbrj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yonumen.top/gthprlyzgx.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gtfjniomqy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jyoumei.cn/gtqtzbrcqz.html

[Q59] 分组内累计
来源：http://hz.zhoulong.xyz/gtsuqtshzt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.feifeiyinyue.top/gtjpsobifv.html

[Q60] 取上一行 / 下一行
来源：http://hz.hywenlv.cn/gtnoeblecp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gtiaehswbv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhijiandao.cn/gtsqqcgtdr.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtofwhplot.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sysykeji.top/gtnhipiprx.html

[Q62] 分组占比
来源：http://hz.tianlin.xyz/gthfgoxxxx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtebonpino.html

[Q63] 开启事务
来源：http://hz.hongshengwenyu.top/gtlqrxcfqs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.0kj1m.cn/gtyrbolwjk.html

[Q64] 提交事务
来源：http://hz.jianghu66.top/gtzwudmujx.html

COMMIT;
来源：http://hz.nanxuanxn.top/gtqgrjvhou.html

[Q65] 回滚事务
来源：http://hz.xuanzx.com/gtmetcwwou.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtalecmpsk.html

[Q66] 行锁查询
来源：http://hz.xingfuxueyuan.xyz/gtbreuaauj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtmyevdbwm.html

[Q67] 设置隔离级别
来源：http://hz.ybcxt.top/gtzszynmlz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtchdtzupm.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtdojyrtcy.html

SAVEPOINT sp1;
来源：http://hz.yongpay.top/gtzdpiwgwh.html

ROLLBACK TO sp1;
来源：http://hz.zhiwuduotai.top/gtpzvqujpf.html

[Q69] 查看执行计划
来源：http://hz.ivvv.top/gtqunbihab.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.0kj1m.cn/gtspmtesnw.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangtech.top/gtmgngsigt.html

ANALYZE TABLE users;
来源：http://hz.yvedp.cn/gtvteqhgai.html

[Q71] 查看建表语句
来源：http://hz.chenlongwang.top/gtexnsoqjp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aibaodan.cn/gtyfuyfrek.html

[Q72] 查看索引
来源：http://hz.yongpay.top/gtsmovgpjj.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtaibqremg.html

[Q73] 查看表状态
来源：http://hz.jiagoushi.top/gtfkkaglix.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhiwuduotai.top/gtwhfpdmjp.html

[Q74] 强制使用索引
来源：http://hz.gotoacloud.top/gtcvsccjxd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnqzz.top/gtidkgucxu.html

[Q75] 日期格式化
来源：http://hz.yvedp.cn/gtdnjtkatr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yueranfly.top/gtgvvkasje.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aibaodan.cn/gttmwfigfd.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtjaqohoto.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.feifeiyinyue.top/gtbitcuqhe.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtadmihxks.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shanyushiyangkeji.top/gttyjnbrfw.html

[Q78] 当前时间
来源：http://hz.dashuyun.cn/gtvgvjkwdo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zdqjudy.top/gtruipcrlu.html

[Q79] 字符串拼接
来源：http://hz.haohaochexian.top/gtdetajjix.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenlongwang.top/gtbrykcjdw.html

[Q80] 字符串截取
来源：http://hz.yuanzhike.top/gtfrjzfand.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jiagoushi.top/gtnpnyntzy.html

[Q81] 字符串替换
来源：http://hz.quarkkingdee.top/gtmgfxkhri.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cheryme.top/gtbzmgqexi.html

[Q82] 字符长度与字节长度
来源：http://hz.pengpengdd.cyou/gtfesvnlcu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj202588.top/gtndazllbw.html

[Q83] 大小写转换
来源：http://hz.shuidangran.top/gtbvgjmmtg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fengsongda.top/gtkowblnks.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gtqvnwflec.html

SELECT TRIM(name) FROM users;
来源：http://hz.cheryme.top/gtplfbvbry.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtkwgvzjxj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yueranfly.top/gtuflunuzn.html

[Q86] 读取 JSON 字段
来源：http://hz.ivvv.top/gtjtmmpieg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.redwolf501.top/gtxwtlnjmx.html

[Q87] JSON 字段做条件
来源：http://hz.haohaochexian.top/gtwnwrgqec.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pycfn.com/gtdusecqid.html

[Q88] 行转列（条件聚合）
来源：http://hz.shuidangran.top/gtblfkvohw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.iojbl.cn/gtxjdlskli.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daxiang520.top/gtgiuukcoa.html

[Q89] 判断表是否存在
来源：http://hz.guowangkeji.top/gtvhfzapol.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.bjfxy.top/gtrinjmyrc.html

[Q90] 生成序号列
来源：http://hz.chenzaomai.com/gtorlituhz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydjk.org.cn/gtvanlluux.html

================================================================================
来源：http://hz.zycfv.cn/gtphuxwocf.html

R. Bash 专题
来源：http://hz.yuxming.cn/gtcbsodjiz.html

================================================================================
来源：http://hz.redwolf501.top/gteoudgbmy.html

[R01] shebang 与严格模式
来源：http://hz.shangyingyoupin.top/gtrkncwoss.html

#!/usr/bin/env bash
来源：http://hz.andypj.xyz/gtdjddmsjt.html

set -euo pipefail
来源：http://hz.mhx1999.top/gtxinosxol.html

[R02] 变量赋值与使用
来源：http://hz.guowangkeji.top/gtetmajgif.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gtztynmcdc.html

[R03] 只读变量
来源：http://hz.gzhubu.top/gtnslpydqw.html

readonly PI=3.14
来源：http://hz.kuanghao11.cn/gtzxugxiva.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtupfjbelq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhongyouzk.top/gtzhgcanyx.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gttxvadwzu.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gtmxucnoys.html

[R06] 判断命令是否存在
来源：http://hz.sxryk.cn/gtgvuvurss.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jyoumei.cn/gtdajspgmo.html

[R07] if 判断文件
来源：http://hz.tianlin.xyz/gtuaqqhtjf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ehwqpu.com/gtmaoubkic.html

[R08] 数值比较
来源：http://hz.zhoulong.xyz/gtjnjxeumx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenjidiqi.icu/gturpocaaz.html

[R09] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gtjczxyimk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.0kj1m.cn/gtsnnchakt.html

[R10] 正则匹配
来源：http://hz.316326.xyz/gtqlzlhezy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.meibo888.top/gtvqpmotwt.html

[R11] case 多分支
来源：http://hz.wangshuangyany.cn/gtycyvuylj.html

case "$1" in
来源：http://hz.yvedp.cn/gttopljpqa.html

start) echo "启动" ;;
来源：http://hz.wangshuangyany.cn/gtqmanvogc.html

stop)  echo "停止" ;;
来源：http://hz.gzhubu.top/gteyexackf.html

*)     echo "未知命令" ;;
来源：http://hz.havefunace.top/gtajwrvgqh.html

esac
来源：http://hz.wangdashe.top/gtwqxxyclb.html

[R12] for 遍历文件
来源：http://hz.jinghuilouyu.cn/gthnulrupw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cheryme.top/gtlddagjbs.html

[R13] for 计数循环
来源：http://hz.zhongyouzk.top/gtptlxpqgj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258888.top/gtxssgbkhx.html

[R14] C 风格 for
来源：http://hz.dashuyun.cn/gtvpbhdvmm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.redwolf501.top/gtftdnxlux.html

[R15] while 逐行读文件
来源：http://hz.ydzc1.top/gtamjubfdp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guannengcc.top/gtdninfuga.html

[R16] until 等待条件
来源：http://hz.svipenyu.cn/gtfjmitwam.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dashuyun.cn/gtfxdpizfb.html

[R17] 数组定义与取值
来源：http://hz.hongshengwenyu.top/gtzqotuipn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.dashuyun.cn/gtpqywrdos.html

[R18] 遍历数组
来源：http://hz.cheryme.top/gtutioovci.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aibaodan.cn/gtbzzurhlc.html

[R19] 数组长度
来源：http://hz.jianghu66.top/gtvnkcnutr.html

echo "${#arr[@]}"
来源：http://hz.yueranfly.top/gtkzeihyty.html

[R20] 关联数组（字典）
来源：http://hz.guowangkeji.top/gtsoryfiki.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aizwys.cn/gtpaskjpxi.html

[R21] 字符串长度
来源：http://hz.pengpengdd.cyou/gtkrdvznay.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtiifzgyvs.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtiutzaoxz.html

echo "${s:0:5}"
来源：http://hz.ivvv.top/gtasnhxkni.html

[R23] 字符串替换
来源：http://hz.xylfe.cn/gtqakajqmf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yongpay.top/gthqtreleq.html

[R24] 大小写转换
来源：http://hz.ybcxt.top/gtjzggvltv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yongpay.top/gtsjnqxqaj.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangshuangyany.cn/gtvpiervmz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gtkxhdczxo.html

[R26] 命令替换
来源：http://hz.chenjidiqi.icu/gtxlkxhfxh.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgufenzy.top/gtctvwohkj.html

[R27] 算术展开
来源：http://hz.9152youxi.cn/gtgcioxqpn.html

echo $((1 + 2 * 3))
来源：http://hz.xuetiantiany.cn/gtvqvhgsaq.html

[R28] 浮点运算
来源：http://hz.jiagoushi.top/gteboqastc.html

echo "scale=2; 10/3" | bc
来源：http://hz.9152youxi.cn/gtcjooaktg.html

[R29] 定义函数
来源：http://hz.wangshuangyany.cn/gtxykhgwkq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gthfyxviqc.html

[R30] 函数返回状态码
来源：http://hz.ydzc1.top/gtrxutyadh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gotoacloud.top/gtpfshitze.html

[R31] 局部变量
来源：http://hz.zhongyouzk.top/gtjkyfbwpb.html

f() { local x=1; echo "$x"; }
来源：http://hz.zdqjudy.top/gtdtwwtzks.html

[R32] 参数个数校验
来源：http://hz.fzhhl.top/gtogwqddxj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtxsrhchho.html

[R33] 捕获错误并提示行号
来源：http://hz.zycfv.cn/gtdryzctbt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgufenzy.top/gtjabsrltl.html

[R34] 退出时清理
来源：http://hz.nanxinkj.top/gtnybzekty.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtyzixykom.html

[R35] 后台执行并等待
来源：http://hz.zhaomingkeji.xyz/gtrhtbystm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhixingplan.top/gtmfvmiijt.html

[R36] 并发执行多个任务
来源：http://hz.xziqi.cn/gtpeyqzjsl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtnwhesmie.html

[R37] 把输出赋给变量
来源：http://hz.gzhubu.top/gtpvylngex.html

files=$(ls -1)
来源：http://hz.gaohongyu789.top/gtayakxrsz.html

[R38] 管道串联
来源：http://hz.jyoumei.cn/gtlvloengz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.0kj1m.cn/gtdffqzmgw.html

[R39] 重定向标准输出与错误
来源：http://hz.wangshuangyany.cn/gtkqcunldw.html

cmd > out.log 2>&1
来源：http://hz.guowangkeji.top/gtjgayeztx.html

[R40] 追加写日志
来源：http://hz.yueranfly.top/gtcxvbkmdf.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtcrdnygbd.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtsomurels.html

cmd >/dev/null 2>&1
来源：http://hz.snrcjt.cn/gtswtaurmc.html

[R42] 输入重定向
来源：http://hz.cashguo.top/gtjgcmjmcy.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtowtewmoj.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtsovfjlbu.html

find . -name "*.log" -type f
来源：http://hz.zhijiandao.cn/gtnpjzlgrf.html

[R44] 按修改时间查找
来源：http://hz.zdqjudy.top/gtxgwfimob.html

find . -mtime -7 -type f
来源：http://hz.jinghuilouyu.cn/gtvaypzqdb.html

[R45] 批量删除
来源：http://hz.birdmap.top/gtlztbyssi.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtsxguulun.html

[R46] 递归替换文件内容
来源：http://hz.zhengqikj.top/gthfkmbatj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtclnyzdyu.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gtbaomshcx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pengpengdd.cyou/gtrdbklwgr.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtuikbboaf.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtrpvlvuvj.html

[R49] awk 带条件
来源：http://hz.chenzaomai.com/gtqqggdhyg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtvpaaulxk.html

[R50] awk 求和
来源：http://hz.havefunace.top/gtmnustwyn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sysykeji.top/gttzpehvnw.html

[R51] 排序去重取前几
来源：http://hz.aibaodan.cn/gtxblpgwzc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.svipenyu.cn/gtcmsfmdbk.html

[R52] 统计行数
来源：http://hz.svipenyu.cn/gtkggyiraz.html

wc -l a.txt
来源：http://hz.kuanghao11.cn/gtauywweku.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtygwddtjs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhiwuduotai.top/gtuukylskw.html

[R54] 比较两个文件
来源：http://hz.hywenlv.cn/gtmerlnpaj.html

diff a.txt b.txt
来源：http://hz.hnxiangtu.top/gtuuoadkbp.html

[R55] 压缩与解压
来源：http://hz.nwbrower.top/gtylkbljwl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gtasouhwje.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtqiggwtem.html

scp file user@host:/path/
来源：http://hz.nanxuanxn.top/gtgbxxdduh.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangkeji.top/gtkanjtugy.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtromwxlvj.html

[R58] 下载文件
来源：http://hz.shzxlz.cn/gtbpgocmgf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtwpiebgyl.html

[R59] 发 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtmkzcakld.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtrrdpwgae.html

[R60] 只看 HTTP 状态码
来源：http://hz.jiagoushi.top/gtcwmfwwrr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtubzqtzsl.html

[R61] 磁盘占用
来源：http://hz.yongpay.top/gtyzdiwcjn.html

df -h;  du -sh *
来源：http://hz.snrcjt.cn/gtpykzxbkh.html

[R62] 找最占空间的文件
来源：http://hz.xziqi.cn/gtzhphhphm.html

du -ah . | sort -rh | head -10
来源：http://hz.havefunace.top/gtbkzhpvxf.html

[R63] 内存与进程
来源：http://hz.gaohongyu789.top/gtgdhgzils.html

free -h;  ps aux | grep nginx
来源：http://hz.ppjwa.cn/gtrginazmv.html

[R64] 结束进程
来源：http://hz.jinyuanbaomall.cn/gtovbcltrl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jlsjyb.cn/gtbipcceei.html

[R65] 查看端口占用
来源：http://hz.yueranfly.top/gtamtmmeje.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cucudq.cn/gtjrxiagfr.html

[R66] 定时任务
来源：http://hz.xingfuxueyuan.xyz/gtwdimvpuo.html

crontab -e;  crontab -l
来源：http://hz.316326.xyz/gtyofiieoy.html

[R67] 生成随机十六进制串
来源：http://hz.cheryme.top/gtaapgqsrd.html

openssl rand -hex 16
来源：http://hz.yangfankeji.com/gtfevyzxju.html

[R68] 计算文件校验值
来源：http://hz.daxiang520.top/gtndeqkito.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hongshengwenyu.top/gtfkznjqda.html

[R69] 生成随机密码
来源：http://hz.cheryme.top/gtdemqjoie.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenjidiqi.icu/gtwezrpcdu.html

[R70] 时间戳与互转
来源：http://hz.nanxinkj.top/gtpammyryr.html

date +%s;  date -d @1700000000
来源：http://hz.xuetiantiany.cn/gttjsmjddo.html

[R71] 日期格式化
来源：http://hz.snrcjt.cn/gtksgymbuk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gogol.net.cn/gttfnzxpkz.html

[R72] 等待端口就绪
来源：http://hz.ivvv.top/gtfkcxxrrg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj202588.top/gtmrhtugft.html

[R73] 分割大日志
来源：http://hz.hysaishi.cn/gtysnizfmr.html

split -l 1000 big.log part_
来源：http://hz.ehwqpu.com/gtchxdqshs.html

[R74] 批量重命名
来源：http://hz.316326.xyz/gtastrvlwt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.vqdsnc.cn/gtwxifeoix.html

[R75] 导出环境变量
来源：http://hz.zycfv.cn/gtfsdccgcj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinghuilouyu.cn/gtwfzqccwz.html

[R76] 使用临时文件
来源：http://hz.zdqjudy.top/gtlylwevdr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtlilphrns.html

[R77] 读取用户输入
来源：http://hz.zhijiandao.cn/gtabwvicus.html

read -rp "请输入: " ans
来源：http://hz.yuxming.cn/gtsmetduzx.html

[R78] 交互式菜单
来源：http://hz.nwbrower.top/gtlvrwqpru.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtdedutilf.html

[R79] 解析命令行选项
来源：http://hz.xylfe.cn/gtmpleubtz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sysykeji.top/gtxgdivtsr.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangtech.top/gtjnyfkyzu.html

time ./run.sh
来源：http://hz.wangdashe.top/gtmvfcoteb.html

================================================================================
来源：http://hz.iojbl.cn/gthstvgaso.html

S. C / C++ 专题
来源：http://hz.chenjidiqi.icu/gtommenkon.html

================================================================================
来源：http://hz.nanxinkj.top/gtwvqlwpow.html

[S01] C：Hello World
来源：http://hz.pengpengdd.cyou/gtwdbembln.html

#include <stdio.h>
来源：http://hz.andypj.xyz/gtvjvqoiir.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj202588.top/gtrknflmvb.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtqpanqyrz.html

int a = 10; printf("%d\n", a);
来源：http://hz.ywan-chungtsiang.top/gtrojzbyya.html

[S03] C：读入整数
来源：http://hz.sufxvd.cn/gtftgngsdd.html

int x; scanf("%d", &x);
来源：http://hz.chenlongwang.top/gtbcmxxvvz.html

[S04] C：字符串复制
来源：http://hz.nwbrower.top/gthlgueytq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yanxiufei.cn/gtohjsrqpn.html

[S05] C：字符串长度
来源：http://hz.ivvv.top/gtvgtngzzb.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gtiyvmuezj.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gteywrmslr.html

strcmp(a, b) == 0
来源：http://hz.zhijiandao.cn/gtzwrdknfi.html

[S07] C：数组遍历求和
来源：http://hz.ehwqpu.com/gtlwpkaety.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cheryme.top/gtbbozalmj.html

[S08] C：动态内存分配与释放
来源：http://hz.xziqi.cn/gtofcqpkcp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tianlin.xyz/gtkxbyznau.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtgelegdpa.html


<!-- 参考信息 -->