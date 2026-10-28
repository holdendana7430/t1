代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hfpthk.cn/gtiqludrix.html

[Q30] 分组统计
来源：http://hz.zhoulong.xyz/gteoyqnwkq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtngzvbryy.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gtioymlega.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hongshengwenyu.top/gtujyoqsgb.html

[Q32] 分组拼接字符串
来源：http://hz.zhengqikj.top/gtdblwulpp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gthfloztjz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fengsongda.top/gtsrjmalqc.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtizdlrpyg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenzaomai.com/gttvxplduy.html

[Q34] 每组取第一条
来源：http://hz.smart0.xyz/gttkvzkdrf.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gtmcvafpnh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yuxming.cn/gtuchfzviq.html

) t WHERE rn = 1;
来源：http://hz.redwolf501.top/gtjgzscdjs.html

[Q35] 内连接
来源：http://hz.yj20258888.top/gtspdzfatn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtmawhzzek.html

[Q36] 左连接
来源：http://hz.wangdashe.top/gtkhoezcgj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtfyzmeqbm.html

[Q37] 右连接
来源：http://hz.jianghu66.top/gtpladznkw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuanzx.com/gtvjoqzizk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinqigfzy.top/gtugoztadi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.kuanghao11.cn/gtfpyzysfl.html

[Q39] 自连接（查上下级）
来源：http://hz.daxiang520.top/gtbmoqhsuz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.bjfxy.top/gtupbgfjfb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gtsykmxpno.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yvedp.cn/gtyvcrcdfr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yuxming.cn/gtmemezllq.html

[Q41] 多表连接
来源：http://hz.shzxlz.cn/gtejadsqyt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ppjwa.cn/gtrsvnhmir.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hfpthk.cn/gtbzklmxkw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ivvv.top/gtrbreffwm.html

[Q42] 连接条件附加过滤
来源：http://hz.yuanzhike.top/gtyqstwhbp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jyoumei.cn/gtkxvhkdyq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258.top/gtsrxtclma.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtsmfdteib.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtofxlgddh.html

[Q44] IN 子查询
来源：http://hz.hysaishi.cn/gtqmulcfux.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jyoumei.cn/gtnhalvikq.html

[Q45] EXISTS 判断存在
来源：http://hz.yvedp.cn/gtqyekmpyh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.vqdsnc.cn/gtabcwpbhn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gzhubu.top/gtytiqhsym.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtkonnjbeq.html

[Q47] 与平均值比较
来源：http://hz.xuetiantiany.cn/gtazykdcms.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.andypj.xyz/gtfelusjvo.html

[Q48] CTE 公用表表达式
来源：http://hz.jianghu66.top/gtorqrwjgm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hfpthk.cn/gtqsqrmkhh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hammf.cn/gtrnxscpgw.html

[Q49] 更新单行
来源：http://hz.hnxiangtu.top/gtnxgwgsjy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pycfn.com/gtgmcewqis.html

[Q50] 批量更新
来源：http://hz.sweek.top/gtgdmsqart.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenlongwang.top/gtzhwtvnnk.html

[Q51] 用子查询更新
来源：http://hz.haohaochexian.top/gtyzfuqpmz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shangyingyoupin.top/gtmplmoudi.html

[Q52] 删除指定行
来源：http://hz.pengpengdd.cyou/gtwyozhvtx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydzc1.top/gtvxuiifqs.html

[Q53] 按条件删除
来源：http://hz.zhixingplan.top/gtyplzwtza.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dashuyun.cn/gtmyjmkdri.html

[Q54] 清空表
来源：http://hz.ydzc1.top/gtebbomsim.html

TRUNCATE TABLE logs;
来源：http://hz.ivvv.top/gtopdpzood.html

[Q55] 排名（并列占位）
来源：http://hz.aizwys.cn/gtjbvqseoi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hfpthk.cn/gtfcntyeds.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenzaomai.com/gtiseyhrjt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yangfankeji.com/gtrjdlkyhy.html

[Q57] 行号
来源：http://hz.gogol.net.cn/gtvmkjovob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daxiang520.top/gtkkgrashg.html

[Q58] 累计求和
来源：http://hz.jinqigufen.top/gtfcrjtldo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yongpay.top/gtsdtrwles.html

[Q59] 分组内累计
来源：http://hz.gotoacloud.top/gtpcrtkwpa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tanke756.top/gthtyunvrx.html

[Q60] 取上一行 / 下一行
来源：http://hz.andypj.xyz/gtbqeeymwy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nanxinkj.top/gtnaykqsqc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtacxujsxw.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gtqrqvnqyg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gtjkwzzqmi.html

[Q62] 分组占比
来源：http://hz.shzxlz.cn/gtxlasimgj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtzxoqkshb.html

[Q63] 开启事务
来源：http://hz.yuanzhike.top/gttochhdmt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtfeksrbil.html

[Q64] 提交事务
来源：http://hz.gaohongyu789.top/gtnzkhxzcj.html

COMMIT;
来源：http://hz.dianchejie.cn/gtyxpaolpe.html

[Q65] 回滚事务
来源：http://hz.zhiwuduotai.top/gtfpdrmsmm.html

ROLLBACK;
来源：http://hz.vqdsnc.cn/gtdjknbpnn.html

[Q66] 行锁查询
来源：http://hz.zhixingplan.top/gthojqwlow.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tian-w.cn/gtowhvwcxg.html

[Q67] 设置隔离级别
来源：http://hz.yj202588.top/gtcxnvwboz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hammf.cn/gtsedszcpn.html

[Q68] 保存点
来源：http://hz.aibaodan.cn/gtbblxnuae.html

SAVEPOINT sp1;
来源：http://hz.xuetiantiany.cn/gtfheorocd.html

ROLLBACK TO sp1;
来源：http://hz.jqgufenzy.top/gtxzecogzc.html

[Q69] 查看执行计划
来源：http://hz.52xcode.cn/gtsfonfppo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.vqdsnc.cn/gtryowjymq.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtwdnpsmpl.html

ANALYZE TABLE users;
来源：http://hz.cashguo.top/gtleumpszd.html

[Q71] 查看建表语句
来源：http://hz.jiagoushi.top/gtqqbjfesx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhoulong.xyz/gtcktswobk.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtastoxryq.html

SHOW INDEX FROM users;
来源：http://hz.vqdsnc.cn/gtzspohirq.html

[Q73] 查看表状态
来源：http://hz.chenlongwang.top/gthgiaefle.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydzc1.top/gtaqeiehza.html

[Q74] 强制使用索引
来源：http://hz.ppjwa.cn/gtqamscghb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.c1oappe.top/gtcykwmabu.html

[Q75] 日期格式化
来源：http://hz.hnxiangtu.top/gtwkseupbu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hnxiangtu.top/gtiphopcse.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yongpay.top/gtkonitzse.html

[Q76] 按天统计
来源：http://hz.kuanghao11.cn/gtrupwkigp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtygizhrox.html

[Q77] 时间加减
来源：http://hz.ydjk.org.cn/gthuzjbluk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtgzcymyew.html

[Q78] 当前时间
来源：http://hz.fengsongda.top/gtpotwayxn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.c1oappe.top/gtbbhhgxqf.html

[Q79] 字符串拼接
来源：http://hz.gzhubu.top/gtyjjxckbm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gotoacloud.top/gttuyojdzc.html

[Q80] 字符串截取
来源：http://hz.fzhhl.top/gtfvjgwlav.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangshuangyany.cn/gtmlmxfzgi.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gttcmbltfz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenjidiqi.icu/gtlwavbvwj.html

[Q82] 字符长度与字节长度
来源：http://hz.vqdsnc.cn/gturhuqotq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.havefunace.top/gtyhsimlvw.html

[Q83] 大小写转换
来源：http://hz.aizwys.cn/gttaauynha.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.316326.xyz/gtjnuabbqj.html

[Q84] 去除首尾空格
来源：http://hz.daria6918.cn/gtdmkvyyzb.html

SELECT TRIM(name) FROM users;
来源：http://hz.kuanghao11.cn/gtqhtulazn.html

[Q85] 数值取整
来源：http://hz.zdqjudy.top/gthtadlnvk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gthfkuziym.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtzhemzgkt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yangfankeji.com/gtjwkgugdl.html

[Q87] JSON 字段做条件
来源：http://hz.xuetiantiany.cn/gtmjpkiepx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yvedp.cn/gtgqmreznd.html

[Q88] 行转列（条件聚合）
来源：http://hz.jiagoushi.top/gtlsezjtfq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daria6918.cn/gtskliifpt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangtech.top/gtthgnklwa.html

[Q89] 判断表是否存在
来源：http://hz.snrcjt.cn/gthnapusnr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.snrcjt.cn/gttlgsaxva.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtljacybvm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydjk.org.cn/gtdzjeirsj.html

================================================================================
来源：http://hz.haohaochexian.top/gtdptgxwsm.html

R. Bash 专题
来源：http://hz.chenzaomai.com/gtmjlxissa.html

================================================================================
来源：http://hz.chenlongwang.top/gtqipdjciw.html

[R01] shebang 与严格模式
来源：http://hz.xuetiantiany.cn/gtbhplmcvf.html

#!/usr/bin/env bash
来源：http://hz.xingfuxueyuan.xyz/gtpaigllmu.html

set -euo pipefail
来源：http://hz.birdmap.top/gtocptleea.html

[R02] 变量赋值与使用
来源：http://hz.aibaodan.cn/gttrszzfmy.html

name="Tom"; echo "$name"
来源：http://hz.yj202588.top/gtljdolcmz.html

[R03] 只读变量
来源：http://hz.andypj.xyz/gtrqhyshwt.html

readonly PI=3.14
来源：http://hz.fengsongda.top/gtbkvwgsfq.html

[R04] 位置参数
来源：http://hz.hnxiangtu.top/gtlyudxpmv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.mhx1999.top/gttavegetf.html

[R05] 参数默认值
来源：http://hz.feifeiyinyue.top/gtxfvrdqwe.html

name="${1:-default}"
来源：http://hz.gotoacloud.top/gtskrhgvmb.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtnsqutibw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fengsongda.top/gtnjqafrpo.html

[R07] if 判断文件
来源：http://hz.hammf.cn/gteckegkpd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ehwqpu.com/gthgwdulpx.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gtvgcikavt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nwbrower.top/gtnsldoezf.html

[R09] 字符串比较
来源：http://hz.bjfxy.top/gtxpnfomts.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.havefunace.top/gtiywfwwhy.html

[R10] 正则匹配
来源：http://hz.yj20258.top/gtessjuavg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guannengcc.top/gtpztkhhhw.html

[R11] case 多分支
来源：http://hz.chenlongwang.top/gtzyanqcet.html

case "$1" in
来源：http://hz.xuanzx.com/gthqihwbzn.html

start) echo "启动" ;;
来源：http://hz.svipenyu.cn/gthpaogals.html

stop)  echo "停止" ;;
来源：http://hz.jianghu66.top/gtscgjrxoz.html

*)     echo "未知命令" ;;
来源：http://hz.smart0.xyz/gtytpfknua.html

esac
来源：http://hz.shzxlz.cn/gtnzmauprb.html

[R12] for 遍历文件
来源：http://hz.tianlin.xyz/gtffhbdrwr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtifmdbant.html

[R13] for 计数循环
来源：http://hz.cheryme.top/gtvhxmfbum.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.guowangkeji.top/gtmthctfwl.html

[R14] C 风格 for
来源：http://hz.meibo888.top/gtynofpcad.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zdqjudy.top/gteppctzdt.html

[R15] while 逐行读文件
来源：http://hz.tian-w.cn/gtxiaoqlxp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigufen.top/gtyathrpyo.html

[R16] until 等待条件
来源：http://hz.birdmap.top/gtxoadlmeo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yuanzhike.top/gtonwbxlgm.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangkeji.top/gtjlmjvbnn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258.top/gtrwfnjmam.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gtxmgfypoh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guowangkeji.top/gtbaasrqfv.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtvycemefw.html

echo "${#arr[@]}"
来源：http://hz.sysykeji.top/gtwiigjdsu.html

[R20] 关联数组（字典）
来源：http://hz.jlsjyb.cn/gtroynsirv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ywan-chungtsiang.top/gtsdpqzzhx.html

[R21] 字符串长度
来源：http://hz.shangyingyoupin.top/gteamtilmi.html

echo "${#s}"
来源：http://hz.birdmap.top/gtfqyxcyxy.html

[R22] 截取子串
来源：http://hz.chenjidiqi.icu/gtylxdquxj.html

echo "${s:0:5}"
来源：http://hz.sufxvd.cn/gtqxzsewfx.html

[R23] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtxqjzfzhu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gogol.net.cn/gtsdaloivy.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gtnehtmzcl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhoulong.xyz/gthgxpvisp.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258888.top/gtdvmecago.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aibaodan.cn/gthkqgczlm.html

[R26] 命令替换
来源：http://hz.zhongyouzk.top/gtbsrdlhsv.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxinkj.top/gtucvncagu.html

[R27] 算术展开
来源：http://hz.xingfuxueyuan.xyz/gtjuzvrula.html

echo $((1 + 2 * 3))
来源：http://hz.yonumen.top/gtbqyrjess.html

[R28] 浮点运算
来源：http://hz.haohaochexian.top/gtbatpbtik.html

echo "scale=2; 10/3" | bc
来源：http://hz.shzxlz.cn/gtjusrzdds.html

[R29] 定义函数
来源：http://hz.zhiwuduotai.top/gtqozvvwdu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gtfkxtbcqc.html

[R30] 函数返回状态码
来源：http://hz.xziqi.cn/gtzgvcybjl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fengsongda.top/gtkpdxnzce.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gthvgzsumk.html

f() { local x=1; echo "$x"; }
来源：http://hz.yvedp.cn/gtpjzpngwh.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gtzmtpdqrn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj202588.top/gtewmpjlgi.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtlhguuthj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhoulong.xyz/gtfkpdcruk.html

[R34] 退出时清理
来源：http://hz.tianlin.xyz/gtyxiztnhx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtyoekpjpc.html

[R35] 后台执行并等待
来源：http://hz.tanke756.top/gtlpjpkjek.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtmtumeogr.html

[R36] 并发执行多个任务
来源：http://hz.yj20258888.top/gtrzbpptap.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenjidiqi.icu/gtctgneuov.html

[R37] 把输出赋给变量
来源：http://hz.redwolf501.top/gtouwxlmyb.html

files=$(ls -1)
来源：http://hz.fengsongda.top/gtyjajtyju.html

[R38] 管道串联
来源：http://hz.nwbrower.top/gtdtozptqr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtzevngpll.html

[R39] 重定向标准输出与错误
来源：http://hz.bjfxy.top/gtuguodojo.html

cmd > out.log 2>&1
来源：http://hz.nwbrower.top/gtjhcuwxoq.html

[R40] 追加写日志
来源：http://hz.jinqigufen.top/gtprojabsy.html

echo "log" >> out.log
来源：http://hz.shuidangran.top/gtzffdrrbp.html

[R41] 丢弃输出
来源：http://hz.cashguo.top/gtbrehpqsd.html

cmd >/dev/null 2>&1
来源：http://hz.ydzc1.top/gtfqitjqtv.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtxcbitfhx.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gthyjvrliu.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtgvnujllk.html

find . -name "*.log" -type f
来源：http://hz.pycfn.com/gtjxeykmra.html

[R44] 按修改时间查找
来源：http://hz.chenjidiqi.icu/gtbvtecuay.html

find . -mtime -7 -type f
来源：http://hz.ybcxt.top/gtakjodmsp.html

[R45] 批量删除
来源：http://hz.ywan-chungtsiang.top/gtkarvhscj.html

find . -name "*.tmp" -delete
来源：http://hz.hongshengwenyu.top/gtwsbdkano.html

[R46] 递归替换文件内容
来源：http://hz.xuetiantiany.cn/gtvdrdpkxp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.0kj1m.cn/gtjazbquoz.html

[R47] sed 单行替换
来源：http://hz.xinyue.icu/gtbrjyvuco.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuanzhike.top/gtltyiovqn.html

[R48] awk 取指定列
来源：http://hz.sxryk.cn/gtmkponhsm.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnxiangtu.top/gtttspbdoh.html

[R49] awk 带条件
来源：http://hz.hnxiangtu.top/gtbbawjbqy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.bjfxy.top/gtuxdyvzig.html

[R50] awk 求和
来源：http://hz.cqqwz.cn/gttogsnieq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gtzbhrkexn.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtxibmncag.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtssyggulm.html

[R52] 统计行数
来源：http://hz.tian-w.cn/gtglivbbht.html

wc -l a.txt
来源：http://hz.daria6918.cn/gtwpfdhcqw.html

[R53] 查看文件头与实时尾
来源：http://hz.xylfe.cn/gthyeuheom.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhongyouzk.top/gtnfnkpgti.html

[R54] 比较两个文件
来源：http://hz.yangfankeji.com/gtnrnesthe.html

diff a.txt b.txt
来源：http://hz.pycfn.com/gtbrwphjze.html

[R55] 压缩与解压
来源：http://hz.ydzc1.top/gtafwpsyte.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guannengcc.top/gtfixaddso.html

[R56] 远程拷贝
来源：http://hz.zhengqikj.top/gtliwnuqxi.html

scp file user@host:/path/
来源：http://hz.jianghu66.top/gtzmyuseqd.html

[R57] 远程执行命令
来源：http://hz.chenjidiqi.icu/gtdfbuoyka.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gtovyzqjsa.html

[R58] 下载文件
来源：http://hz.daxiang520.top/gtyqcmupzj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangshuangyany.cn/gtfzcqrkdb.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangtech.top/gtgykkxpfd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gttvheapug.html

[R60] 只看 HTTP 状态码
来源：http://hz.xinyue.icu/gtafcdivin.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xziqi.cn/gtbisnxhkb.html

[R61] 磁盘占用
来源：http://hz.shuidangran.top/gtvfkuqwkx.html

df -h;  du -sh *
来源：http://hz.zdqjudy.top/gtvapkslox.html

[R62] 找最占空间的文件
来源：http://hz.aizwys.cn/gttwlymvca.html

du -ah . | sort -rh | head -10
来源：http://hz.ppjwa.cn/gtrrebkinw.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtfkvzhymd.html

free -h;  ps aux | grep nginx
来源：http://hz.birdmap.top/gtyedywdpy.html

[R64] 结束进程
来源：http://hz.quarkkingdee.top/gtlikgvfyf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ybcxt.top/gtdomzxtqh.html

[R65] 查看端口占用
来源：http://hz.aizwys.cn/gtrlpsjubf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.smart0.xyz/gtjaractci.html

[R66] 定时任务
来源：http://hz.redwolf501.top/gtrweppyrl.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gtdqojrolv.html

[R67] 生成随机十六进制串
来源：http://hz.hnxiangtu.top/gtjasqdvws.html

openssl rand -hex 16
来源：http://hz.iojbl.cn/gtosaudnar.html

[R68] 计算文件校验值
来源：http://hz.feifeiyinyue.top/gtvnigjtub.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhoulong.xyz/gtcbbaokqd.html

[R69] 生成随机密码
来源：http://hz.hnxiangtu.top/gtaskdcfyz.html

head -c 16 /dev/urandom | base64
来源：http://hz.0kj1m.cn/gtzdxheall.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtxznqozxn.html

date +%s;  date -d @1700000000
来源：http://hz.cheryme.top/gtandkbijb.html

[R71] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtqszkdhcw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pengpengdd.cyou/gtoraykcox.html

[R72] 等待端口就绪
来源：http://hz.ppjwa.cn/gtverdkhxt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtmrfaoksl.html

[R73] 分割大日志
来源：http://hz.xylfe.cn/gtdgfaobdz.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangtech.top/gtmcenvtry.html

[R74] 批量重命名
来源：http://hz.chenlongwang.top/gtlpwzswrw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtpyiemiwl.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtxhetdqgn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gtgsgcxwxp.html

[R76] 使用临时文件
来源：http://hz.yongpay.top/gtjzvlsdju.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtwkecxgiy.html

[R77] 读取用户输入
来源：http://hz.ppjwa.cn/gtjtuheyyk.html

read -rp "请输入: " ans
来源：http://hz.mhx1999.top/gtizbsoelf.html

[R78] 交互式菜单
来源：http://hz.dashuyun.cn/gtcdwwklmw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.52xcode.cn/gtveuaybva.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gtifpxsevs.html


<!-- 参考信息 -->