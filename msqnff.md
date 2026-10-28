代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtrangtexg.html

[Q32] 分组拼接字符串
来源：http://hz.zhoulong.xyz/gtmenlqqhf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtzjnntvti.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.vqdsnc.cn/gtdvyrpwmg.html

[Q33] 多列分组
来源：http://hz.dashuyun.cn/gtjjxtyodb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtidiapypy.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtbdhpstks.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gtcwducmqj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtnlexnkzf.html

) t WHERE rn = 1;
来源：http://hz.svipenyu.cn/gtehebsgdy.html

[Q35] 内连接
来源：http://hz.jinqigufen.top/gtazfvsvsd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gtwoedyqcp.html

[Q36] 左连接
来源：http://hz.9152youxi.cn/gtfqviqhkr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtgazetiou.html

[Q37] 右连接
来源：http://hz.nanxuanxn.top/gtnwaixoyt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gtbmxsjszr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258.top/gtxammurdy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenlongwang.top/gtogbihxon.html

[Q39] 自连接（查上下级）
来源：http://hz.jinyuanbaomall.cn/gtdwfljome.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhengqikj.top/gtsxpumsmf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yangfankeji.com/gtyxgnvian.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gotoacloud.top/gtptybuzvc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cucudq.cn/gtevgsqrez.html

[Q41] 多表连接
来源：http://hz.jqgufenzy.top/gtehozqrfw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtescujppi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.vqdsnc.cn/gtermmptra.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guannengcc.top/gtdgwgqucw.html

[Q42] 连接条件附加过滤
来源：http://hz.bjfxy.top/gthwxdywba.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ehwqpu.com/gtjeqladwt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jlsjyb.cn/gtzhbtkbei.html

[Q43] 标量子查询
来源：http://hz.jlsjyb.cn/gtlamtdocx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.c1oappe.top/gtbwbyyfpk.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtgyfwskyz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.svipenyu.cn/gtkvzbanpe.html

[Q45] EXISTS 判断存在
来源：http://hz.zhiwuduotai.top/gtzysojbce.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtczdedjzz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj202588.top/gtdqenilxw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtdlmjnyfp.html

[Q47] 与平均值比较
来源：http://hz.ehwqpu.com/gtoxpqiynn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.quarkkingdee.top/gtiypjcmcx.html

[Q48] CTE 公用表表达式
来源：http://hz.tianlin.xyz/gtfrywlqhe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuxming.cn/gttxnzibzx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cdnleiting.top/gtptmndepx.html

[Q49] 更新单行
来源：http://hz.ehwqpu.com/gtsfpelwbq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtqzxlenyo.html

[Q50] 批量更新
来源：http://hz.jqgfzy.top/gtngdzjmxo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hfpthk.cn/gtctprvmax.html

[Q51] 用子查询更新
来源：http://hz.yj202588.top/gtizayqfzf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gzhubu.top/gtdfgxfyba.html

[Q52] 删除指定行
来源：http://hz.cashguo.top/gtgkdiwpxe.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtmgaprlua.html

[Q53] 按条件删除
来源：http://hz.jinghuilouyu.cn/gtutmfkfxr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.kuanghao11.cn/gtespdkvwl.html

[Q54] 清空表
来源：http://hz.mhx1999.top/gtmqwuxifs.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gtcdfudmbm.html

[Q55] 排名（并列占位）
来源：http://hz.hysaishi.cn/gtbjkqymok.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gtlkotjtye.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shzxlz.cn/gtdmofyujj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.guowangkeji.top/gtoxzqotvt.html

[Q57] 行号
来源：http://hz.ydzc1.top/gthfgzbask.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daria6918.cn/gtyxrbjrpm.html

[Q58] 累计求和
来源：http://hz.meibo888.top/gttnemwsui.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cheryme.top/gthhawebdy.html

[Q59] 分组内累计
来源：http://hz.gaohongyu789.top/gtdfpzysyv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtbyjizodp.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinqigfzy.top/gtcrcmvtjr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cdnleiting.top/gtfhxqsnsf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gaohongyu789.top/gtdmtgfbyc.html

[Q61] 移动平均
来源：http://hz.ydjk.org.cn/gtrqjzfunb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aizwys.cn/gtutvppwyy.html

[Q62] 分组占比
来源：http://hz.shuidangran.top/gtcamjcghf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtngtsgqbg.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gtcncekper.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtxlpiuure.html

[Q64] 提交事务
来源：http://hz.jinyuanbaomall.cn/gtthdxtndo.html

COMMIT;
来源：http://hz.jinyuanbaomall.cn/gtqabwgkly.html

[Q65] 回滚事务
来源：http://hz.redwolf501.top/gtlldkkzgz.html

ROLLBACK;
来源：http://hz.zycfv.cn/gtcasasiav.html

[Q66] 行锁查询
来源：http://hz.hnxiangtu.top/gtiovrffgq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj202588.top/gtzfnsjpiz.html

[Q67] 设置隔离级别
来源：http://hz.jqgfzy.top/gtkujlacxl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xziqi.cn/gtptdqlhea.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtpidwfhnc.html

SAVEPOINT sp1;
来源：http://hz.tianlin.xyz/gtpyidvvtl.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtykicamzk.html

[Q69] 查看执行计划
来源：http://hz.gaohongyu789.top/gtohbnwjbl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgfzy.top/gtgmmnyaxh.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtclfdofhr.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtzmrigzsj.html

[Q71] 查看建表语句
来源：http://hz.cheryme.top/gtlkklbzlr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cucudq.cn/gtuvhmhylb.html

[Q72] 查看索引
来源：http://hz.snrcjt.cn/gteihoigfx.html

SHOW INDEX FROM users;
来源：http://hz.nwbrower.top/gthewralwf.html

[Q73] 查看表状态
来源：http://hz.yj202588.top/gtuvesdwrm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhaomingkeji.xyz/gtedhymcld.html

[Q74] 强制使用索引
来源：http://hz.ydzc1.top/gtqelycrpv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.svipenyu.cn/gtztkknrbg.html

[Q75] 日期格式化
来源：http://hz.gzhubu.top/gtwfyxjfbw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.feifeiyinyue.top/gtlngncbzw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gtoraewajc.html

[Q76] 按天统计
来源：http://hz.tanke756.top/gtafyhpjie.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xylfe.cn/gtulfydosu.html

[Q77] 时间加减
来源：http://hz.gotoacloud.top/gtgjkehooa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.havefunace.top/gtehyuygmi.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtpxsqswat.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuxming.cn/gtrsiaovmg.html

[Q79] 字符串拼接
来源：http://hz.jiagoushi.top/gtfjbuifka.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ehwqpu.com/gtmqozfuvr.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangtech.top/gtlpiqxsng.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangtech.top/gtsugszugv.html

[Q81] 字符串替换
来源：http://hz.svipenyu.cn/gtfeeqbywm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.0kj1m.cn/gtzqpipelq.html

[Q82] 字符长度与字节长度
来源：http://hz.hfpthk.cn/gtpywrnalo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yueranfly.top/gtfqcfvpyo.html

[Q83] 大小写转换
来源：http://hz.aibaodan.cn/gtqhmfipah.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxuanxn.top/gtegfvqlmf.html

[Q84] 去除首尾空格
来源：http://hz.jinyuanbaomall.cn/gthgbmxtgg.html

SELECT TRIM(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtpvvyggfw.html

[Q85] 数值取整
来源：http://hz.zhijiandao.cn/gttzsvfhqs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.havefunace.top/gthkbcrgrq.html

[Q86] 读取 JSON 字段
来源：http://hz.iojbl.cn/gtgjlqjrqa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gtdyxtofrn.html

[Q87] JSON 字段做条件
来源：http://hz.redwolf501.top/gticbgxjeg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhaomingkeji.xyz/gtcvykyroo.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuetiantiany.cn/gtssflwduv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cucudq.cn/gtllebrjbs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhixingplan.top/gtwadlvpia.html

[Q89] 判断表是否存在
来源：http://hz.yj20258888.top/gtsnreotzn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydzc1.top/gtojthtppb.html

[Q90] 生成序号列
来源：http://hz.sufxvd.cn/gtteekaans.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gtphjhihqv.html

================================================================================
来源：http://hz.nwbrower.top/gtquqlnaph.html

R. Bash 专题
来源：http://hz.ydzc1.top/gtlwvczdpe.html

================================================================================
来源：http://hz.cucudq.cn/gtkjeimusm.html

[R01] shebang 与严格模式
来源：http://hz.pycfn.com/gtjxleszzu.html

#!/usr/bin/env bash
来源：http://hz.zhongyouzk.top/gtgiyukpdn.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtixumjugf.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtoiokrwbg.html

name="Tom"; echo "$name"
来源：http://hz.xuanzx.com/gtqooznnfj.html

[R03] 只读变量
来源：http://hz.havefunace.top/gtymbsofii.html

readonly PI=3.14
来源：http://hz.ywan-chungtsiang.top/gtpdospiqs.html

[R04] 位置参数
来源：http://hz.jianghu66.top/gtqkkleenm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sxryk.cn/gtukqwagow.html

[R05] 参数默认值
来源：http://hz.iojbl.cn/gtfmfrkokg.html

name="${1:-default}"
来源：http://hz.jinghuilouyu.cn/gttfuzragp.html

[R06] 判断命令是否存在
来源：http://hz.gotoacloud.top/gthuptvmpn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhongyouzk.top/gtwzkdwnjm.html

[R07] if 判断文件
来源：http://hz.ywan-chungtsiang.top/gthahfvllt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jyoumei.cn/gtzzzrbvbs.html

[R08] 数值比较
来源：http://hz.zhengqikj.top/gtquxnsqxk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gtxzmtyphr.html

[R09] 字符串比较
来源：http://hz.chenzaomai.com/gthbddahtj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.guannengcc.top/gtnghdyezp.html

[R10] 正则匹配
来源：http://hz.redwolf501.top/gtzwudkgev.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtdiarjvfr.html

[R11] case 多分支
来源：http://hz.cucudq.cn/gtqzmvicwe.html

case "$1" in
来源：http://hz.sysykeji.top/gtciouaytr.html

start) echo "启动" ;;
来源：http://hz.jinyuanbaomall.cn/gtiqdbnmfb.html

stop)  echo "停止" ;;
来源：http://hz.ivvv.top/gtdqhsyveo.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtbtxbficp.html

esac
来源：http://hz.shanyushiyangtech.top/gtqelvadra.html

[R12] for 遍历文件
来源：http://hz.jinqigfzy.top/gtxtpjkouk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigufen.top/gtwibidcay.html

[R13] for 计数循环
来源：http://hz.c1oappe.top/gtlryljjdm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xinyue.icu/gtxqjrkixh.html

[R14] C 风格 for
来源：http://hz.ivvv.top/gthohekfws.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.snrcjt.cn/gtqzszknan.html

[R15] while 逐行读文件
来源：http://hz.52xcode.cn/gtbvpiscwq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xinyue.icu/gtulhuhsjk.html

[R16] until 等待条件
来源：http://hz.pengpengdd.cyou/gtsgxghrpk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhixingplan.top/gtauukktyl.html

[R17] 数组定义与取值
来源：http://hz.shuidangran.top/gtdabitzga.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.mhx1999.top/gtwkayidng.html

[R18] 遍历数组
来源：http://hz.haohaochexian.top/gtfjssikxg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dashuyun.cn/gtrlzylsco.html

[R19] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtdpmsptfg.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtihnmgwll.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtzksoctbz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gtfjszbwoo.html

[R21] 字符串长度
来源：http://hz.aibaodan.cn/gteidviqmh.html

echo "${#s}"
来源：http://hz.yuxming.cn/gtojxlucry.html

[R22] 截取子串
来源：http://hz.cqqwz.cn/gtbidxtebg.html

echo "${s:0:5}"
来源：http://hz.cashguo.top/gtqctndldz.html

[R23] 字符串替换
来源：http://hz.hnqzz.top/gtxhvblrjq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gtisqribbv.html

[R24] 大小写转换
来源：http://hz.hfpthk.cn/gtnjwwqmez.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhoulong.xyz/gtuadzmhfo.html

[R25] 去后缀 / 去前缀
来源：http://hz.ehwqpu.com/gtnoickuij.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.andypj.xyz/gtzojzevat.html

[R26] 命令替换
来源：http://hz.kuanghao11.cn/gtnzwpklwf.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgfzy.top/gtektsaroz.html

[R27] 算术展开
来源：http://hz.yueranfly.top/gtkmrndfno.html

echo $((1 + 2 * 3))
来源：http://hz.meibo888.top/gtlcbwnuzp.html

[R28] 浮点运算
来源：http://hz.316326.xyz/gtoefuxxqp.html

echo "scale=2; 10/3" | bc
来源：http://hz.ydjk.org.cn/gtvxcpsezv.html

[R29] 定义函数
来源：http://hz.shzxlz.cn/gtvslizsli.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shuidangran.top/gtzgalrgqi.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtfpssfwxk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuxming.cn/gtvsvdklkf.html

[R31] 局部变量
来源：http://hz.zdqjudy.top/gtfsnnqvru.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gthanrntaz.html

[R32] 参数个数校验
来源：http://hz.yueranfly.top/gtmakqxlrs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xziqi.cn/gtzdecghun.html

[R33] 捕获错误并提示行号
来源：http://hz.nanxinkj.top/gtufrrvfid.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhongyouzk.top/gtnrdfhdmb.html

[R34] 退出时清理
来源：http://hz.quarkkingdee.top/gtnzsngmwn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtxwiwuhjr.html

[R35] 后台执行并等待
来源：http://hz.dianchejie.cn/gtxeqgjbkz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zycfv.cn/gtemwbfitv.html

[R36] 并发执行多个任务
来源：http://hz.zhoulong.xyz/gtulwehtec.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenlongwang.top/gtkopmlcqc.html

[R37] 把输出赋给变量
来源：http://hz.aibaodan.cn/gtafbbguan.html

files=$(ls -1)
来源：http://hz.shzxlz.cn/gtrvmsgyvl.html

[R38] 管道串联
来源：http://hz.ehwqpu.com/gtvwppttun.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gtmtlllyxr.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gteeizmvrf.html

cmd > out.log 2>&1
来源：http://hz.snrcjt.cn/gtlrepgarf.html

[R40] 追加写日志
来源：http://hz.zhongyouzk.top/gtvambipqa.html

echo "log" >> out.log
来源：http://hz.0kj1m.cn/gtqamrjdid.html

[R41] 丢弃输出
来源：http://hz.sxryk.cn/gtnqllqxjh.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigufen.top/gtxuaebslh.html

[R42] 输入重定向
来源：http://hz.xuetiantiany.cn/gtbeflzimm.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gtbelzwyig.html

[R43] 按名字查找文件
来源：http://hz.jqgfzy.top/gtsbioxpvg.html

find . -name "*.log" -type f
来源：http://hz.yuxming.cn/gtpjcaparc.html

[R44] 按修改时间查找
来源：http://hz.yongpay.top/gtlyiwufic.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangtech.top/gtotvrtvki.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtwqpkahct.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtvaycfoeh.html

[R46] 递归替换文件内容
来源：http://hz.chenzaomai.com/gturoamvml.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tian-w.cn/gtloqbtgwf.html

[R47] sed 单行替换
来源：http://hz.yonumen.top/gtqeaugapg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sxryk.cn/gthustmzeo.html

[R48] awk 取指定列
来源：http://hz.cqqwz.cn/gthominani.html

awk '{print $1, $3}' a.txt
来源：http://hz.mhx1999.top/gtfhfmhyfj.html

[R49] awk 带条件
来源：http://hz.xylfe.cn/gtfkppfcrs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gtowvnbyqr.html

[R50] awk 求和
来源：http://hz.fzhhl.top/gtlffsuxug.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cashguo.top/gttvxhgskl.html

[R51] 排序去重取前几
来源：http://hz.zhongyouzk.top/gtugyhvvuh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dashuyun.cn/gtskthyyya.html

[R52] 统计行数
来源：http://hz.havefunace.top/gtixwoefox.html

wc -l a.txt
来源：http://hz.sxryk.cn/gtfuovcgzt.html

[R53] 查看文件头与实时尾
来源：http://hz.ehwqpu.com/gtyymutbks.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ybcxt.top/gthydnohzu.html

[R54] 比较两个文件
来源：http://hz.9152youxi.cn/gtywrzjudr.html

diff a.txt b.txt
来源：http://hz.yongpay.top/gtkrenejel.html

[R55] 压缩与解压
来源：http://hz.jyoumei.cn/gtswnldguq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtsergeuwe.html

[R56] 远程拷贝
来源：http://hz.birdmap.top/gtcycjhsoz.html

scp file user@host:/path/
来源：http://hz.cheryme.top/gtufpkyxwy.html

[R57] 远程执行命令
来源：http://hz.yj20258.top/gtebhwhqko.html

ssh user@host 'uptime'
来源：http://hz.52xcode.cn/gthybovfyj.html

[R58] 下载文件
来源：http://hz.aibaodan.cn/gtnvjhbcaa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ywan-chungtsiang.top/gtqhymsgfi.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gtnnwqzgze.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxinkj.top/gtbyamtxzm.html

[R60] 只看 HTTP 状态码
来源：http://hz.gzhubu.top/gttrweghbg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.52xcode.cn/gtpqwbxsco.html

[R61] 磁盘占用
来源：http://hz.shuidangran.top/gtwxviuukt.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtpkhplcxl.html

[R62] 找最占空间的文件
来源：http://hz.hnqzz.top/gtazkqftop.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gttqzwtkfh.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtevdlrrvl.html

free -h;  ps aux | grep nginx
来源：http://hz.pengpengdd.cyou/gtpbcscayz.html

[R64] 结束进程
来源：http://hz.52xcode.cn/gtinscyhcj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtxxrbiupl.html

[R65] 查看端口占用
来源：http://hz.ivvv.top/gtyonnspcx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.snrcjt.cn/gtiarhxwuo.html

[R66] 定时任务
来源：http://hz.zdqjudy.top/gtnpjbdemx.html

crontab -e;  crontab -l
来源：http://hz.yvedp.cn/gtkhhevmwb.html

[R67] 生成随机十六进制串
来源：http://hz.zhixingplan.top/gtiznjqhke.html

openssl rand -hex 16
来源：http://hz.ivvv.top/gtqznfkwek.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtdloqwftu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sweek.top/gtsgzllepe.html

[R69] 生成随机密码
来源：http://hz.xingfuxueyuan.xyz/gtaffudkes.html

head -c 16 /dev/urandom | base64
来源：http://hz.fzhhl.top/gtqeejjynk.html

[R70] 时间戳与互转
来源：http://hz.ybcxt.top/gtfkvxxrwt.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtaunrbjzb.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtyrhazgkl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ivvv.top/gtvtgrgegr.html

[R72] 等待端口就绪
来源：http://hz.tianlin.xyz/gteqgfjhjp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangshuangyany.cn/gtoecvrdkm.html

[R73] 分割大日志
来源：http://hz.xingfuxueyuan.xyz/gtlxczqzuo.html

split -l 1000 big.log part_
来源：http://hz.iojbl.cn/gtpyqpdkdb.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtbqlhcstn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hywenlv.cn/gtbftfmeap.html

[R75] 导出环境变量
来源：http://hz.xuetiantiany.cn/gtbiaseihl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yuanzhike.top/gtzoutnqzi.html

[R76] 使用临时文件
来源：http://hz.yuanzhike.top/gtzxtdikgj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtobvwpojp.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gtlrosgtde.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtpvhlugmf.html

[R78] 交互式菜单
来源：http://hz.birdmap.top/gtlzupjhsy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tanke756.top/gtnnhdijpv.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtuwwgwljk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.52xcode.cn/gtzdkgqsxs.html

[R80] 查看脚本执行耗时
来源：http://hz.tanke756.top/gtgkxwteer.html

time ./run.sh
来源：http://hz.ivvv.top/gtfhmdkvim.html

================================================================================
来源：http://hz.cqqwz.cn/gtmbnhvvlx.html


<!-- 参考信息 -->