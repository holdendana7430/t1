代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtdmkzkppv.html

[Q20] IN 列表
来源：http://hz.tian-w.cn/gtshdwcfut.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnqzz.top/gtyhlwcwhl.html

[Q21] 空值判断
来源：http://hz.smart0.xyz/gtfseuejvx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.meibo888.top/gtdzowlyeu.html

[Q22] 排序
来源：http://hz.gzhubu.top/gtbbldeoxw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhiwuduotai.top/gthwodfyxt.html

[Q23] 分页
来源：http://hz.xuanzx.com/gtwmlguwtc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.52xcode.cn/gtzmwdwwxf.html

[Q24] 去重
来源：http://hz.hammf.cn/gtitqhwdgc.html

SELECT DISTINCT city FROM users;
来源：http://hz.jyoumei.cn/gtqyglgrce.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gtsubnavwv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangtech.top/gtqjdmypio.html

[Q26] 计数
来源：http://hz.yuxming.cn/gtebucuzsx.html

SELECT COUNT(*) FROM users;
来源：http://hz.cashguo.top/gtoruwlwuc.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtripgrosf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dianchejie.cn/gtwslxdwzf.html

[Q28] 求和与平均
来源：http://hz.cheryme.top/gtsxcqswxt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtapvaflwm.html

[Q29] 最大最小值
来源：http://hz.9152youxi.cn/gthjsavtyq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtyemyirjm.html

[Q30] 分组统计
来源：http://hz.wangdashe.top/gtpkvpeipy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtkxjqrefx.html

[Q31] 分组后过滤
来源：http://hz.sysykeji.top/gtvazctfom.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hfpthk.cn/gtjjwcrjet.html

[Q32] 分组拼接字符串
来源：http://hz.zhoulong.xyz/gtcewfoyye.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtyrdnwinl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.haohaochexian.top/gtkbpxaxgx.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtokhdjsof.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xziqi.cn/gtsoustrlx.html

[Q34] 每组取第一条
来源：http://hz.yj202588.top/gtsfcmlmau.html

SELECT * FROM (
来源：http://hz.pycfn.com/gtwizoipdx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shanyushiyangtech.top/gtiozhesjh.html

) t WHERE rn = 1;
来源：http://hz.hnxiangtu.top/gtflnfddfw.html

[Q35] 内连接
来源：http://hz.wangdashe.top/gtxxudwrgh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtjqowmjyb.html

[Q36] 左连接
来源：http://hz.daria6918.cn/gtvrhmzvxk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtpgletmpi.html

[Q37] 右连接
来源：http://hz.redwolf501.top/gtyvnnsfli.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.0kj1m.cn/gtespionqw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ppjwa.cn/gtdhoxagit.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.fengsongda.top/gtrwowbllg.html

[Q39] 自连接（查上下级）
来源：http://hz.zhengqikj.top/gtkkkteecm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gttaepjkrr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.guowangkeji.top/gttfoersup.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj20258888.top/gtfcmwxdgs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jianghu66.top/gtmgwgfmfi.html

[Q41] 多表连接
来源：http://hz.shanyushiyangkeji.top/gtesqbdzbp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yonumen.top/gtjazewzae.html

JOIN users u ON u.id = o.user_id
来源：http://hz.birdmap.top/gtkzjkuase.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gzhubu.top/gtrryiorir.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtlghodjug.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtoycafgbi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jlsjyb.cn/gtsnxniorz.html

[Q43] 标量子查询
来源：http://hz.yangfankeji.com/gtlxqpvcdq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenjidiqi.icu/gtapxpvouy.html

[Q44] IN 子查询
来源：http://hz.zhaomingkeji.xyz/gtcwerpmzu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydjk.org.cn/gtlynvmggj.html

[Q45] EXISTS 判断存在
来源：http://hz.ydzc1.top/gtatcotfem.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtnwtjhxwr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtsviylwgy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtcymvaepu.html

[Q47] 与平均值比较
来源：http://hz.sufxvd.cn/gtdzpypvpb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.fzhhl.top/gtaucuatzk.html

[Q48] CTE 公用表表达式
来源：http://hz.jinghuilouyu.cn/gtcwbvocqd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xziqi.cn/gtaslcamfm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangkeji.top/gtmeeaiubd.html

[Q49] 更新单行
来源：http://hz.zhongyouzk.top/gtvbtebewn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sweek.top/gtknhvzhdd.html

[Q50] 批量更新
来源：http://hz.jqgufenzy.top/gtverkmveh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zdqjudy.top/gtmlsvfyzo.html

[Q51] 用子查询更新
来源：http://hz.shuidangran.top/gtnmnygddg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.andypj.xyz/gtqekucxdk.html

[Q52] 删除指定行
来源：http://hz.kuanghao11.cn/gtdhmsdcrg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gtfgvgfdty.html

[Q53] 按条件删除
来源：http://hz.shangyingyoupin.top/gtnsahyjgk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenzaomai.com/gtlusrxkww.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtborwradt.html

TRUNCATE TABLE logs;
来源：http://hz.yongpay.top/gtzmfjnuyt.html

[Q55] 排名（并列占位）
来源：http://hz.wangshuangyany.cn/gtddeffwnr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ehwqpu.com/gtpndeneoy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtgxtfyfsb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hongshengwenyu.top/gtudgsnruj.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtdyngcbou.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtmxgmvtgw.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gtwiwoqbmu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.svipenyu.cn/gtxnqnstbe.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangkeji.top/gtrydpgmwz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.mhx1999.top/gtwhwdozuv.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj202588.top/gtakicyiau.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ivvv.top/gtztqdaflr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shangyingyoupin.top/gtfabewlwd.html

[Q61] 移动平均
来源：http://hz.wangshuangyany.cn/gtuodmvuct.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhijiandao.cn/gtroqdvzsk.html

[Q62] 分组占比
来源：http://hz.jyoumei.cn/gtkmcokinj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtyhrgcrkb.html

[Q63] 开启事务
来源：http://hz.52xcode.cn/gtlxpcgdju.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtpawtghtb.html

[Q64] 提交事务
来源：http://hz.0kj1m.cn/gtpvqayskr.html

COMMIT;
来源：http://hz.yonumen.top/gtxbumnjxa.html

[Q65] 回滚事务
来源：http://hz.zhiwuduotai.top/gtgbogrbtp.html

ROLLBACK;
来源：http://hz.gotoacloud.top/gtoqrmaoia.html

[Q66] 行锁查询
来源：http://hz.aizwys.cn/gtaisahrot.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xziqi.cn/gtufmyttrc.html

[Q67] 设置隔离级别
来源：http://hz.gogol.net.cn/gtufvwbeaq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.haohaochexian.top/gtnfxzetnh.html

[Q68] 保存点
来源：http://hz.mhx1999.top/gtvqscpgjm.html

SAVEPOINT sp1;
来源：http://hz.iojbl.cn/gtkjcqumpb.html

ROLLBACK TO sp1;
来源：http://hz.svipenyu.cn/gtbnhenztl.html

[Q69] 查看执行计划
来源：http://hz.jinqigufen.top/gtdfshkzip.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhixingplan.top/gtplbdxbnr.html

[Q70] 更新统计信息
来源：http://hz.hnxiangtu.top/gtvdbvinkl.html

ANALYZE TABLE users;
来源：http://hz.yongpay.top/gtcrhjittz.html

[Q71] 查看建表语句
来源：http://hz.andypj.xyz/gtsfduyxup.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtcgumzzdy.html

[Q72] 查看索引
来源：http://hz.nanxinkj.top/gtcxdpmjyr.html

SHOW INDEX FROM users;
来源：http://hz.redwolf501.top/gtnbfvtudo.html

[Q73] 查看表状态
来源：http://hz.vqdsnc.cn/gtnykhbind.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhongyouzk.top/gtpgzjdrrl.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtqdahccjd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gzhubu.top/gtddjlsqdp.html

[Q75] 日期格式化
来源：http://hz.sysykeji.top/gtaoxwiegf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtimcthkuc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ehwqpu.com/gtynosrlgu.html

[Q76] 按天统计
来源：http://hz.ywan-chungtsiang.top/gtonwcfjmw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hysaishi.cn/gtoelzxrox.html

[Q77] 时间加减
来源：http://hz.hysaishi.cn/gtogxjnsqa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258888.top/gtfhqpxays.html

[Q78] 当前时间
来源：http://hz.zhixingplan.top/gtrushafne.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.haohaochexian.top/gtwslndhuh.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtjslbcfhp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gotoacloud.top/gtpfbqwttd.html

[Q80] 字符串截取
来源：http://hz.zhengqikj.top/gtpbhzxcue.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yanxiufei.cn/gtlhodaosy.html

[Q81] 字符串替换
来源：http://hz.aibaodan.cn/gtqbppaxnj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydjk.org.cn/gtnixbsikf.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtfzyrhcla.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sweek.top/gtykcmdsie.html

[Q83] 大小写转换
来源：http://hz.xylfe.cn/gtjewyzuay.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtunfplcci.html

[Q84] 去除首尾空格
来源：http://hz.jyoumei.cn/gtetdsksdw.html

SELECT TRIM(name) FROM users;
来源：http://hz.iojbl.cn/gtzybzoveq.html

[Q85] 数值取整
来源：http://hz.0kj1m.cn/gtbsmfgkya.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gtbxuqoiee.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtjnbsgnes.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gzhubu.top/gtupfgugdp.html

[Q87] JSON 字段做条件
来源：http://hz.tian-w.cn/gtsbgzxlwc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shzxlz.cn/gtaerlysug.html

[Q88] 行转列（条件聚合）
来源：http://hz.meibo888.top/gtjysbmeup.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yonumen.top/gtvoiuiout.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.redwolf501.top/gtmpghstml.html

[Q89] 判断表是否存在
来源：http://hz.yueranfly.top/gthzyvqsfv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cheryme.top/gticddcrhv.html

[Q90] 生成序号列
来源：http://hz.daxiang520.top/gtoiifjpao.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gtuakoctpp.html

================================================================================
来源：http://hz.sufxvd.cn/gtppnsfioc.html

R. Bash 专题
来源：http://hz.zhaomingkeji.xyz/gtuylvhomd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtffluzqrk.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gtcrukyngl.html

#!/usr/bin/env bash
来源：http://hz.wangshuangyany.cn/gtftljfdhr.html

set -euo pipefail
来源：http://hz.xuanzx.com/gtbzkcraye.html

[R02] 变量赋值与使用
来源：http://hz.andypj.xyz/gtifjddprn.html

name="Tom"; echo "$name"
来源：http://hz.zhoulong.xyz/gtskwskfye.html

[R03] 只读变量
来源：http://hz.shzxlz.cn/gtbjglyumm.html

readonly PI=3.14
来源：http://hz.ehwqpu.com/gtjwscmbah.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtkwcvibyj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.kuanghao11.cn/gtwdvfpmkd.html

[R05] 参数默认值
来源：http://hz.gzhubu.top/gtxmwilout.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtjnqifpzu.html

[R06] 判断命令是否存在
来源：http://hz.snrcjt.cn/gtjyyteqzp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnxiangtu.top/gttrsycnne.html

[R07] if 判断文件
来源：http://hz.redwolf501.top/gtsrfplhev.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtaodqqqwn.html

[R08] 数值比较
来源：http://hz.cqqwz.cn/gtrzeaqgwy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tanke756.top/gttupniunb.html

[R09] 字符串比较
来源：http://hz.sweek.top/gtykrxssww.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ybcxt.top/gtfrytmdeo.html

[R10] 正则匹配
来源：http://hz.zhaomingkeji.xyz/gtlnakulby.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258.top/gteyghnhbs.html

[R11] case 多分支
来源：http://hz.pengpengdd.cyou/gtdgqwhibl.html

case "$1" in
来源：http://hz.hnxiangtu.top/gtkfxfcpsx.html

start) echo "启动" ;;
来源：http://hz.gotoacloud.top/gthacrpidw.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtvqoiwqir.html

*)     echo "未知命令" ;;
来源：http://hz.ydjk.org.cn/gttkpslhoo.html

esac
来源：http://hz.haohaochexian.top/gtqiifjhot.html

[R12] for 遍历文件
来源：http://hz.xuanzx.com/gtipzhqyhy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtndblnzfj.html

[R13] for 计数循环
来源：http://hz.chenjidiqi.icu/gtltsrwjxj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtcuisgxru.html

[R14] C 风格 for
来源：http://hz.yueranfly.top/gtvymsjubv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtnryqpfej.html

[R15] while 逐行读文件
来源：http://hz.xuanzx.com/gtgyveyugc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinyuanbaomall.cn/gtitxoolbz.html

[R16] until 等待条件
来源：http://hz.nwbrower.top/gtzeffudxq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gtuvjfjial.html

[R17] 数组定义与取值
来源：http://hz.jinqigfzy.top/gtgzqaywqe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daria6918.cn/gtexgjgpkr.html

[R18] 遍历数组
来源：http://hz.yj20258.top/gtkxkstrdg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hongshengwenyu.top/gtufgjsrrr.html

[R19] 数组长度
来源：http://hz.cucudq.cn/gtrnetqtiq.html

echo "${#arr[@]}"
来源：http://hz.ivvv.top/gtjiqmnowz.html

[R20] 关联数组（字典）
来源：http://hz.pycfn.com/gttpgjvcss.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.havefunace.top/gtzmrzwxgb.html

[R21] 字符串长度
来源：http://hz.sweek.top/gtagmuytxs.html

echo "${#s}"
来源：http://hz.tianlin.xyz/gtlhrxhgim.html

[R22] 截取子串
来源：http://hz.hongshengwenyu.top/gthozxpchc.html

echo "${s:0:5}"
来源：http://hz.sxryk.cn/gtsturongx.html

[R23] 字符串替换
来源：http://hz.aibaodan.cn/gtopjpvzhu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nwbrower.top/gtiavkjqvb.html

[R24] 大小写转换
来源：http://hz.zhengqikj.top/gtwcajnpdq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cheryme.top/gtxhuxhqlv.html

[R25] 去后缀 / 去前缀
来源：http://hz.0kj1m.cn/gtaiutrxyg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtlqqaeoqg.html

[R26] 命令替换
来源：http://hz.hysaishi.cn/gtknvtdpve.html

now=$(date +%F); echo "$now"
来源：http://hz.yvedp.cn/gtwtndewgb.html

[R27] 算术展开
来源：http://hz.tian-w.cn/gtatinmtzt.html

echo $((1 + 2 * 3))
来源：http://hz.ydzc1.top/gtfnwwftjk.html

[R28] 浮点运算
来源：http://hz.zhengqikj.top/gtzmqmmjdy.html

echo "scale=2; 10/3" | bc
来源：http://hz.guowangkeji.top/gtyyxqlpsv.html

[R29] 定义函数
来源：http://hz.pengpengdd.cyou/gtcaurxhkg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.9152youxi.cn/gtzdbksmfm.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtgmnyejmt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtlnywpqjs.html

[R31] 局部变量
来源：http://hz.nanxinkj.top/gtxpmruqdb.html

f() { local x=1; echo "$x"; }
来源：http://hz.cheryme.top/gtttftrvfz.html

[R32] 参数个数校验
来源：http://hz.sysykeji.top/gtpadnriqq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtveflktyr.html

[R33] 捕获错误并提示行号
来源：http://hz.gzhubu.top/gtoykjxtml.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guowangkeji.top/gtwvwxlhzp.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtzfoazyue.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtlkkdgnnb.html

[R35] 后台执行并等待
来源：http://hz.sxryk.cn/gtmsitmgfx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cucudq.cn/gtbpjzsfiz.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtmosfnaug.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jiagoushi.top/gtabwvmbxq.html

[R37] 把输出赋给变量
来源：http://hz.ybcxt.top/gtcapsakod.html

files=$(ls -1)
来源：http://hz.52xcode.cn/gthggpaxwd.html

[R38] 管道串联
来源：http://hz.meibo888.top/gtyggdwiks.html

cat a.txt | grep -i error | wc -l
来源：http://hz.andypj.xyz/gtpujehuyl.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtglgdppvk.html

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtbpemahiw.html

[R40] 追加写日志
来源：http://hz.jinyuanbaomall.cn/gtszjgvoek.html

echo "log" >> out.log
来源：http://hz.jinyuanbaomall.cn/gtojjyybeu.html

[R41] 丢弃输出
来源：http://hz.cqqwz.cn/gthjlbbbtz.html

cmd >/dev/null 2>&1
来源：http://hz.yuxming.cn/gtzligbldq.html

[R42] 输入重定向
来源：http://hz.haohaochexian.top/gtfhcrnyhd.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtawrddnlz.html

[R43] 按名字查找文件
来源：http://hz.hfpthk.cn/gtevjyfzjf.html

find . -name "*.log" -type f
来源：http://hz.hywenlv.cn/gtzlmkoeie.html

[R44] 按修改时间查找
来源：http://hz.ehwqpu.com/gtgekbcelc.html

find . -mtime -7 -type f
来源：http://hz.hnqzz.top/gtddokmyca.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gthuutawxc.html

find . -name "*.tmp" -delete
来源：http://hz.hongshengwenyu.top/gtecjyxixq.html

[R46] 递归替换文件内容
来源：http://hz.sysykeji.top/gtjqimqurp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhixingplan.top/gtwnlogbeh.html

[R47] sed 单行替换
来源：http://hz.0kj1m.cn/gtkvaejsiv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daria6918.cn/gtrokfcyui.html

[R48] awk 取指定列
来源：http://hz.wangdashe.top/gtwrjrusrx.html

awk '{print $1, $3}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtimwvxlri.html

[R49] awk 带条件
来源：http://hz.hammf.cn/gtwdufillm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yangfankeji.com/gtflgcfhpr.html

[R50] awk 求和
来源：http://hz.hongshengwenyu.top/gtnnttnmoq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gtytfxpvtz.html

[R51] 排序去重取前几
来源：http://hz.hnqzz.top/gtlnjryycl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuanzhike.top/gtntqkzdcl.html

[R52] 统计行数
来源：http://hz.zhaomingkeji.xyz/gtfqbleinc.html

wc -l a.txt
来源：http://hz.yangfankeji.com/gthczvuwih.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtlaahuqvb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shuidangran.top/gtbcaechis.html

[R54] 比较两个文件
来源：http://hz.nanxinkj.top/gtxkcugxlq.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtmqtdxybj.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtsannhapm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenzaomai.com/gtyrajzulo.html

[R56] 远程拷贝
来源：http://hz.yj202588.top/gtguoiihiw.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtmcvegiur.html

[R57] 远程执行命令
来源：http://hz.zhoulong.xyz/gtnmbntwvp.html

ssh user@host 'uptime'
来源：http://hz.dashuyun.cn/gtynmffpgf.html

[R58] 下载文件
来源：http://hz.tian-w.cn/gtodclwgxf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhiwuduotai.top/gtoohymupj.html

[R59] 发 POST JSON
来源：http://hz.yvedp.cn/gtgdwwxerr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.52xcode.cn/gtcsxvqhwf.html

[R60] 只看 HTTP 状态码
来源：http://hz.pycfn.com/gtpyhtsjsp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangkeji.top/gtrmwekxpq.html

[R61] 磁盘占用
来源：http://hz.cheryme.top/gtlgxlnwzs.html

df -h;  du -sh *
来源：http://hz.cqqwz.cn/gtcbsgdquv.html

[R62] 找最占空间的文件
来源：http://hz.jlsjyb.cn/gtqfvdotzi.html

du -ah . | sort -rh | head -10
来源：http://hz.chenjidiqi.icu/gtkevdozci.html

[R63] 内存与进程
来源：http://hz.haohaochexian.top/gtbekuhzod.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxuanxn.top/gtjxalvllh.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gtzvhqenut.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtztzktcfr.html

[R65] 查看端口占用
来源：http://hz.hongshengwenyu.top/gtkssfuhlm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gtrxbwwqah.html

[R66] 定时任务
来源：http://hz.9152youxi.cn/gtozgkfsly.html

crontab -e;  crontab -l
来源：http://hz.tanke756.top/gtmktscxwz.html

[R67] 生成随机十六进制串
来源：http://hz.ivvv.top/gtyvnjvnmd.html

openssl rand -hex 16
来源：http://hz.shangyingyoupin.top/gtgfrtkpds.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtqatqyhgp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gaohongyu789.top/gthhhmhjtb.html

[R69] 生成随机密码
来源：http://hz.yj202588.top/gtdgeaggwl.html


<!-- 参考信息 -->