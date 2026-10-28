代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxinkj.top/gtsuwsujdf.html

[Q32] 分组拼接字符串
来源：http://hz.kuanghao11.cn/gtvoyjgybt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtmrwyitik.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnxiangtu.top/gtxuwojfyv.html

[Q33] 多列分组
来源：http://hz.yongpay.top/gttabahcdy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gotoacloud.top/gtjxfrpgba.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtqhxhjhms.html

SELECT * FROM (
来源：http://hz.zycfv.cn/gtrtjtbrxp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtugnjcjek.html

) t WHERE rn = 1;
来源：http://hz.xuetiantiany.cn/gtneqjsipd.html

[Q35] 内连接
来源：http://hz.cashguo.top/gtscsmkrkc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gtqtqgibbm.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtmcyyzgxf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtqpzboxdf.html

[Q37] 右连接
来源：http://hz.meibo888.top/gtvephwrwm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtwlcsimjv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yongpay.top/gtoascvhkl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cqqwz.cn/gtsnivtkkv.html

[Q39] 自连接（查上下级）
来源：http://hz.wangdashe.top/gtikuukvwk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuetiantiany.cn/gtbdqwtese.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258888.top/gttvnvfupy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhiwuduotai.top/gtkknlgvvv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtbpnimfrj.html

[Q41] 多表连接
来源：http://hz.c1oappe.top/gtkdvmgvbn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.birdmap.top/gtfflzyvwm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gtfvkckdnc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinyuanbaomall.cn/gtwncqjgab.html

[Q42] 连接条件附加过滤
来源：http://hz.shangyingyoupin.top/gtxzmjzjaf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yongpay.top/gtjrgjzrvc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.bjfxy.top/gtpnwdfstg.html

[Q43] 标量子查询
来源：http://hz.jqgufenzy.top/gtrryqmzde.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhijiandao.cn/gtlnuzacoz.html

[Q44] IN 子查询
来源：http://hz.hysaishi.cn/gtvnryxfxe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yuxming.cn/gtbgtokdfg.html

[Q45] EXISTS 判断存在
来源：http://hz.zycfv.cn/gtnizgjzav.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daxiang520.top/gttsmfrwcv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fengsongda.top/gtancytkra.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daxiang520.top/gtyrqsrgby.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtbdvveyen.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangdashe.top/gthpfxasub.html

[Q48] CTE 公用表表达式
来源：http://hz.hywenlv.cn/gtqegbrdkz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.snrcjt.cn/gtqvttglpt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigufen.top/gtnmowyvuh.html

[Q49] 更新单行
来源：http://hz.iojbl.cn/gtehmcrzuv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtygahvtuz.html

[Q50] 批量更新
来源：http://hz.shanyushiyangtech.top/gthqulosbv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhongyouzk.top/gteowovena.html

[Q51] 用子查询更新
来源：http://hz.jinyuanbaomall.cn/gtuhwytijy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenlongwang.top/gtgfpjppsl.html

[Q52] 删除指定行
来源：http://hz.birdmap.top/gtlefcwhal.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtalslhcuq.html

[Q53] 按条件删除
来源：http://hz.daria6918.cn/gttvqetsge.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhoulong.xyz/gtpvxbpmnb.html

[Q54] 清空表
来源：http://hz.dianchejie.cn/gttfqngmyp.html

TRUNCATE TABLE logs;
来源：http://hz.ehwqpu.com/gtvpynhqpe.html

[Q55] 排名（并列占位）
来源：http://hz.cqqwz.cn/gtqaxgabwm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sweek.top/gtebdwmyli.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuetiantiany.cn/gtwqgbgydn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gtdrzskaem.html

[Q57] 行号
来源：http://hz.yvedp.cn/gtgagqoqai.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.iojbl.cn/gtucbpcooa.html

[Q58] 累计求和
来源：http://hz.birdmap.top/gtkultgfcs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tianlin.xyz/gtzwdhcwbu.html

[Q59] 分组内累计
来源：http://hz.xinyue.icu/gtpswxbfax.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gtyujvxops.html

[Q60] 取上一行 / 下一行
来源：http://hz.gotoacloud.top/gtmmjtuhrn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtgyhwqwtb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuanzx.com/gtpmztqzow.html

[Q61] 移动平均
来源：http://hz.sufxvd.cn/gtkwmxsclp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtxsajpybb.html

[Q62] 分组占比
来源：http://hz.pycfn.com/gtadefkbtp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtyfwhefbs.html

[Q63] 开启事务
来源：http://hz.shzxlz.cn/gteaabnsir.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtvvqqzhvf.html

[Q64] 提交事务
来源：http://hz.zhongyouzk.top/gtbtzveibc.html

COMMIT;
来源：http://hz.shangyingyoupin.top/gtwlygcsvv.html

[Q65] 回滚事务
来源：http://hz.tanke756.top/gtzdlkjfsu.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtvdsbxxpn.html

[Q66] 行锁查询
来源：http://hz.316326.xyz/gtfyglloem.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shuidangran.top/gtiqbgvjbx.html

[Q67] 设置隔离级别
来源：http://hz.xuanzx.com/gtqxfwscml.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangdashe.top/gtfwjlubip.html

[Q68] 保存点
来源：http://hz.tanke756.top/gtycxgdwln.html

SAVEPOINT sp1;
来源：http://hz.ppjwa.cn/gtzljdzvlj.html

ROLLBACK TO sp1;
来源：http://hz.zhoulong.xyz/gtwyrcinqa.html

[Q69] 查看执行计划
来源：http://hz.hongshengwenyu.top/gtxlctubfr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.316326.xyz/gtzhtrfzad.html

[Q70] 更新统计信息
来源：http://hz.xuanzx.com/gtygdfscsu.html

ANALYZE TABLE users;
来源：http://hz.havefunace.top/gtlwaigstb.html

[Q71] 查看建表语句
来源：http://hz.daxiang520.top/gtwwrbfbsg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gtrzuqordt.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gtrdemyptn.html

SHOW INDEX FROM users;
来源：http://hz.zycfv.cn/gtivnoogbr.html

[Q73] 查看表状态
来源：http://hz.cqqwz.cn/gtrcqmmsoc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhoulong.xyz/gtvqibdpcx.html

[Q74] 强制使用索引
来源：http://hz.mhx1999.top/gtydctscuz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.kuanghao11.cn/gthulajuil.html

[Q75] 日期格式化
来源：http://hz.aizwys.cn/gtpbrujdrp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.andypj.xyz/gtjflggnqs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj202588.top/gtwvtslvrl.html

[Q76] 按天统计
来源：http://hz.xuanzx.com/gtseonucqm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuanzx.com/gtncrzyoki.html

[Q77] 时间加减
来源：http://hz.jinqigfzy.top/gtnuuzmvmw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtntcqgqep.html

[Q78] 当前时间
来源：http://hz.tanke756.top/gtguwpbvdl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shuidangran.top/gtyfogmvnl.html

[Q79] 字符串拼接
来源：http://hz.aibaodan.cn/gtzjeknpnf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jianghu66.top/gtneuwwqas.html

[Q80] 字符串截取
来源：http://hz.jqgufenzy.top/gtnatftvys.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuanzhike.top/gtqfdqchkl.html

[Q81] 字符串替换
来源：http://hz.zdqjudy.top/gtwsdmevlu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gttqmbmhmn.html

[Q82] 字符长度与字节长度
来源：http://hz.ywan-chungtsiang.top/gtqacbyuyi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hysaishi.cn/gttekdxxgg.html

[Q83] 大小写转换
来源：http://hz.zhijiandao.cn/gtuocislkr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.redwolf501.top/gtjneqkyte.html

[Q84] 去除首尾空格
来源：http://hz.guannengcc.top/gtpcsvepsg.html

SELECT TRIM(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtspbpzalx.html

[Q85] 数值取整
来源：http://hz.ywan-chungtsiang.top/gtnmlukvog.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jianghu66.top/gtrfekckmq.html

[Q86] 读取 JSON 字段
来源：http://hz.zhixingplan.top/gtrteqlqvo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tian-w.cn/gtmptdjqcx.html

[Q87] JSON 字段做条件
来源：http://hz.chenlongwang.top/gtgzvdobwi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gthwtmayyh.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxinkj.top/gtqwadtsve.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yuxming.cn/gtqjhfkjfr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gtlfjpwocj.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtlnvphxmm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.meibo888.top/gtjleszryy.html

[Q90] 生成序号列
来源：http://hz.tian-w.cn/gtahlpdgvo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tianlin.xyz/gtkffnkkib.html

================================================================================
来源：http://hz.xylfe.cn/gtxxkdvdjn.html

R. Bash 专题
来源：http://hz.yj20258888.top/gtuobtklqa.html

================================================================================
来源：http://hz.zhoulong.xyz/gtczlnuxor.html

[R01] shebang 与严格模式
来源：http://hz.gotoacloud.top/gtmgxuzabx.html

#!/usr/bin/env bash
来源：http://hz.c1oappe.top/gtsabyekhd.html

set -euo pipefail
来源：http://hz.tianlin.xyz/gtijmoncbz.html

[R02] 变量赋值与使用
来源：http://hz.jlsjyb.cn/gttmhfnbop.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gtykvqbomo.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gtvldwuvbb.html

readonly PI=3.14
来源：http://hz.xinyue.icu/gtqtkdzqro.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gttgjievqu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shuidangran.top/gtnvaeuxvm.html

[R05] 参数默认值
来源：http://hz.yongpay.top/gtjyvelhxx.html

name="${1:-default}"
来源：http://hz.shzxlz.cn/gtzqqknjqd.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtnuzmjunu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cashguo.top/gtkohwdene.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtaefibvkh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxuanxn.top/gtawysaflb.html

[R08] 数值比较
来源：http://hz.daria6918.cn/gttofypezr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinghuilouyu.cn/gtmubqpxrd.html

[R09] 字符串比较
来源：http://hz.wangdashe.top/gtsdvdoemg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtxghsqcfw.html

[R10] 正则匹配
来源：http://hz.yuanzhike.top/gttdxxherr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sufxvd.cn/gttrtlgdcf.html

[R11] case 多分支
来源：http://hz.chenjidiqi.icu/gtjybnnwre.html

case "$1" in
来源：http://hz.ywan-chungtsiang.top/gtgpliexpc.html

start) echo "启动" ;;
来源：http://hz.quarkkingdee.top/gtggtczehd.html

stop)  echo "停止" ;;
来源：http://hz.jiagoushi.top/gtmfuywysg.html

*)     echo "未知命令" ;;
来源：http://hz.tian-w.cn/gtzymkijsw.html

esac
来源：http://hz.ywan-chungtsiang.top/gtklararlm.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtqjobklqy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sxryk.cn/gtjjawjkko.html

[R13] for 计数循环
来源：http://hz.meibo888.top/gtqzxtfdmo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gthpfydmtk.html

[R14] C 风格 for
来源：http://hz.cucudq.cn/gtdfkgjfpt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenlongwang.top/gthmujmnjh.html

[R15] while 逐行读文件
来源：http://hz.xuanzx.com/gtbvxlqxhp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xziqi.cn/gttmddfpir.html

[R16] until 等待条件
来源：http://hz.wangshuangyany.cn/gthzvyhxhm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.0kj1m.cn/gttitgbjvg.html

[R17] 数组定义与取值
来源：http://hz.yanxiufei.cn/gtneuopkfl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.0kj1m.cn/gtyvojhkab.html

[R18] 遍历数组
来源：http://hz.tianlin.xyz/gtbiwbscud.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuetiantiany.cn/gtsgrmuggl.html

[R19] 数组长度
来源：http://hz.jlsjyb.cn/gtubmasqlu.html

echo "${#arr[@]}"
来源：http://hz.jqgfzy.top/gttzkvayar.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtwzswqpmi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gtozaonzcn.html

[R21] 字符串长度
来源：http://hz.feifeiyinyue.top/gtyoipppfv.html

echo "${#s}"
来源：http://hz.tian-w.cn/gtvmcqpeyh.html

[R22] 截取子串
来源：http://hz.yuanzhike.top/gtldpmqxoj.html

echo "${s:0:5}"
来源：http://hz.aizwys.cn/gttikzdgmh.html

[R23] 字符串替换
来源：http://hz.jinghuilouyu.cn/gttvacmcxv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guannengcc.top/gtgsyopsbk.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtovqyeqgn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daxiang520.top/gtmgaphcwu.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtzgryqfve.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.mhx1999.top/gtjccpbnlb.html

[R26] 命令替换
来源：http://hz.hammf.cn/gtomhetscq.html

now=$(date +%F); echo "$now"
来源：http://hz.wangshuangyany.cn/gtrjjxrkdp.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtonfkxttl.html

echo $((1 + 2 * 3))
来源：http://hz.ivvv.top/gtkckfqxsb.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtibutzloo.html

echo "scale=2; 10/3" | bc
来源：http://hz.cheryme.top/gtohororwo.html

[R29] 定义函数
来源：http://hz.guowangkeji.top/gtdyuwrtyj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gzhubu.top/gtacnaddmf.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtqigbtsjs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zycfv.cn/gtglfvndhc.html

[R31] 局部变量
来源：http://hz.pycfn.com/gtdmsnjeeh.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gtgdciaoey.html

[R32] 参数个数校验
来源：http://hz.daxiang520.top/gtxmzgczqy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gttljtsvci.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gtzjgtdiok.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtevnsrnzh.html

[R34] 退出时清理
来源：http://hz.yj202588.top/gtaqydxufh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtwatkvoni.html

[R35] 后台执行并等待
来源：http://hz.yanxiufei.cn/gtrvcvpink.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhijiandao.cn/gtgrztnpwd.html

[R36] 并发执行多个任务
来源：http://hz.yonumen.top/gtqxykfjwu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.quarkkingdee.top/gtynwpzksp.html

[R37] 把输出赋给变量
来源：http://hz.zhaomingkeji.xyz/gtgkjdwcca.html

files=$(ls -1)
来源：http://hz.quarkkingdee.top/gtrcnbatct.html

[R38] 管道串联
来源：http://hz.guowangkeji.top/gtjarfzqob.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yongpay.top/gtmejmqleo.html

[R39] 重定向标准输出与错误
来源：http://hz.jianghu66.top/gtshuamfro.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtqywsmdym.html

[R40] 追加写日志
来源：http://hz.jqgufenzy.top/gtiwboepqu.html

echo "log" >> out.log
来源：http://hz.yj20258888.top/gtlcdpewxd.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtdfgvwrba.html

cmd >/dev/null 2>&1
来源：http://hz.chenzaomai.com/gtkfvyqefs.html

[R42] 输入重定向
来源：http://hz.vqdsnc.cn/gtjnqgtpaw.html

wc -l < a.txt
来源：http://hz.haohaochexian.top/gtplrnunsk.html

[R43] 按名字查找文件
来源：http://hz.andypj.xyz/gtdbymtdko.html

find . -name "*.log" -type f
来源：http://hz.wangshuangyany.cn/gtfnpjreji.html

[R44] 按修改时间查找
来源：http://hz.hammf.cn/gtighpmzxk.html

find . -mtime -7 -type f
来源：http://hz.gaohongyu789.top/gtowqunsuf.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gtgtyrdsqw.html

find . -name "*.tmp" -delete
来源：http://hz.xuanzx.com/gtbyljrszs.html

[R46] 递归替换文件内容
来源：http://hz.gaohongyu789.top/gtjjldjkku.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aibaodan.cn/gtvnlbuqoj.html

[R47] sed 单行替换
来源：http://hz.tianlin.xyz/gtzxcbgzgv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenjidiqi.icu/gtpfzrykux.html

[R48] awk 取指定列
来源：http://hz.jinghuilouyu.cn/gthkqdnwwk.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gtazdhkhjh.html

[R49] awk 带条件
来源：http://hz.bjfxy.top/gtbhixfiik.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daria6918.cn/gtkgrscaux.html

[R50] awk 求和
来源：http://hz.shanyushiyangkeji.top/gtznyzqwij.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhixingplan.top/gtdbifdajb.html

[R51] 排序去重取前几
来源：http://hz.zhoulong.xyz/gtpkodvcyw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hysaishi.cn/gtfebtvvdz.html

[R52] 统计行数
来源：http://hz.zhijiandao.cn/gtiopnuvqr.html

wc -l a.txt
来源：http://hz.xylfe.cn/gteyuaqtju.html

[R53] 查看文件头与实时尾
来源：http://hz.iojbl.cn/gtrnfnbfth.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenjidiqi.icu/gtxefkxpjn.html

[R54] 比较两个文件
来源：http://hz.havefunace.top/gtrfqtcjjo.html

diff a.txt b.txt
来源：http://hz.zdqjudy.top/gtnsvvcqjo.html

[R55] 压缩与解压
来源：http://hz.jiagoushi.top/gthwwcisno.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cheryme.top/gtfpoavqpk.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtflvaovvq.html

scp file user@host:/path/
来源：http://hz.nanxinkj.top/gttlppafwr.html

[R57] 远程执行命令
来源：http://hz.andypj.xyz/gttlybwczc.html

ssh user@host 'uptime'
来源：http://hz.yuanzhike.top/gtnctsayra.html

[R58] 下载文件
来源：http://hz.bjfxy.top/gtkvzydery.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gogol.net.cn/gtfyecjmlh.html

[R59] 发 POST JSON
来源：http://hz.c1oappe.top/gtiasogiqu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtviwzhvto.html

[R60] 只看 HTTP 状态码
来源：http://hz.ydzc1.top/gtbggiwkui.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dashuyun.cn/gtfivfpyge.html

[R61] 磁盘占用
来源：http://hz.hammf.cn/gtwlunrsil.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gttqqoyous.html

[R62] 找最占空间的文件
来源：http://hz.sufxvd.cn/gtgnqxdshw.html

du -ah . | sort -rh | head -10
来源：http://hz.52xcode.cn/gtklnhgiyi.html

[R63] 内存与进程
来源：http://hz.aibaodan.cn/gtqygpfnje.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gtwsmpfxpg.html

[R64] 结束进程
来源：http://hz.gotoacloud.top/gthmbuinic.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sxryk.cn/gtngdpmzev.html

[R65] 查看端口占用
来源：http://hz.0kj1m.cn/gtabybmgnh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nanxuanxn.top/gtmucoipih.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtqmohitqg.html

crontab -e;  crontab -l
来源：http://hz.ppjwa.cn/gtoiflvjjg.html

[R67] 生成随机十六进制串
来源：http://hz.haohaochexian.top/gtwevkvxxs.html

openssl rand -hex 16
来源：http://hz.jinyuanbaomall.cn/gtreypzqum.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangkeji.top/gtufqwbjqy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangkeji.top/gtxikhyfsb.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtsrzwkxzr.html

head -c 16 /dev/urandom | base64
来源：http://hz.fzhhl.top/gtgnmjaimb.html

[R70] 时间戳与互转
来源：http://hz.xingfuxueyuan.xyz/gtlecrwmjd.html

date +%s;  date -d @1700000000
来源：http://hz.shanyushiyangkeji.top/gtjvvpxlqc.html

[R71] 日期格式化
来源：http://hz.xuanzx.com/gthzfskevq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.feifeiyinyue.top/gtyhyksilf.html

[R72] 等待端口就绪
来源：http://hz.52xcode.cn/gtpgdtxdxj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtlufitlzj.html

[R73] 分割大日志
来源：http://hz.birdmap.top/gtpayjncbz.html

split -l 1000 big.log part_
来源：http://hz.kuanghao11.cn/gtwntwabti.html

[R74] 批量重命名
来源：http://hz.hnqzz.top/gturbubdzv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cashguo.top/gtswciwjqc.html

[R75] 导出环境变量
来源：http://hz.wangshuangyany.cn/gtlnnzglza.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.vqdsnc.cn/gthitvedwm.html

[R76] 使用临时文件
来源：http://hz.tanke756.top/gtxfqrkmdq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtpodaugrv.html

[R77] 读取用户输入
来源：http://hz.jqgfzy.top/gtjhltbeqg.html

read -rp "请输入: " ans
来源：http://hz.ywan-chungtsiang.top/gtkgvqrprn.html

[R78] 交互式菜单
来源：http://hz.cdnleiting.top/gtvomwrqro.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.52xcode.cn/gtfmdfdzmj.html

[R79] 解析命令行选项
来源：http://hz.daxiang520.top/gtawnpjokd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.meibo888.top/gttvvmzcji.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtckrmyhuy.html

time ./run.sh
来源：http://hz.jinghuilouyu.cn/gtgwxrfnyt.html

================================================================================
来源：http://hz.snrcjt.cn/gtlmfxhhfq.html


<!-- 参考信息 -->