代发 wailian999

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtkdfnzzpj.html

[Q16] 查询指定列
来源：http://hz.jinqigfzy.top/gtnqkjcvcs.html

SELECT id, name FROM users;
来源：http://hz.wangdashe.top/gtoidnzhrt.html

[Q17] 条件查询
来源：http://hz.yj202588.top/gtuedlzdal.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj20258888.top/gtutxutaus.html

[Q18] 模糊匹配
来源：http://hz.fengsongda.top/gtymmhouwq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangshuangyany.cn/gtawsklnmb.html

[Q19] 范围查询
来源：http://hz.cheryme.top/gtzlhmpseh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gotoacloud.top/gtwreamgnx.html

[Q20] IN 列表
来源：http://hz.haohaochexian.top/gtomqfaumq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.iojbl.cn/gtdlgnxndb.html

[Q21] 空值判断
来源：http://hz.ivvv.top/gtgmhiqzsj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuxming.cn/gtpyuiqfyg.html

[Q22] 排序
来源：http://hz.chenlongwang.top/gtuwprrjrv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jlsjyb.cn/gtovzmtlel.html

[Q23] 分页
来源：http://hz.zhixingplan.top/gtfubrnpem.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guannengcc.top/gthvaccgmg.html

[Q24] 去重
来源：http://hz.316326.xyz/gthnywbvlt.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtswrrqnub.html

[Q25] 只取前 N 条
来源：http://hz.xinyue.icu/gtmvlkwmfp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhixingplan.top/gtzcfwenum.html

[Q26] 计数
来源：http://hz.yvedp.cn/gtdwbjhjtw.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtsdxexlvg.html

[Q27] 条件计数
来源：http://hz.quarkkingdee.top/gtixkzjxau.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hammf.cn/gtcirkbsby.html

[Q28] 求和与平均
来源：http://hz.gotoacloud.top/gtbpbykowx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yongpay.top/gtzftskuvu.html

[Q29] 最大最小值
来源：http://hz.vqdsnc.cn/gtzeangdxi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gtllqwajhb.html

[Q30] 分组统计
来源：http://hz.zhiwuduotai.top/gtigsqerex.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtfqzkkmtv.html

[Q31] 分组后过滤
来源：http://hz.sufxvd.cn/gtxwhlztlj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yueranfly.top/gtsqfppxkl.html

[Q32] 分组拼接字符串
来源：http://hz.sxryk.cn/gtvshwxvcz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtkrvhrjwi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.bjfxy.top/gtjgedruwr.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtcnixvgsj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.andypj.xyz/gtakjqzvpx.html

[Q34] 每组取第一条
来源：http://hz.wangdashe.top/gtesvtejiu.html

SELECT * FROM (
来源：http://hz.gotoacloud.top/gtitbbluio.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gtqlfougle.html

) t WHERE rn = 1;
来源：http://hz.sxryk.cn/gtijksfqkn.html

[Q35] 内连接
来源：http://hz.aibaodan.cn/gtussnpkfn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtxkjvohsg.html

[Q36] 左连接
来源：http://hz.sxryk.cn/gtckkdxepk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jiagoushi.top/gtkbedemdk.html

[Q37] 右连接
来源：http://hz.yangfankeji.com/gtcziwmdxx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhengqikj.top/gtadzuuark.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtteavisdy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.smart0.xyz/gtqndsgfwr.html

[Q39] 自连接（查上下级）
来源：http://hz.andypj.xyz/gtbbonqvqo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigfzy.top/gtvmprqxmd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yongpay.top/gtwbvodgsv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aizwys.cn/gtehmhpujw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tanke756.top/gtffhzwjmb.html

[Q41] 多表连接
来源：http://hz.iojbl.cn/gtlvqwuhao.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nwbrower.top/gtuocpljxk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.vqdsnc.cn/gtlhyspnwy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jianghu66.top/gtobjhdlfq.html

[Q42] 连接条件附加过滤
来源：http://hz.ydzc1.top/gtehzdaoao.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtaorkjnuf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daxiang520.top/gtchdxnsag.html

[Q43] 标量子查询
来源：http://hz.gaohongyu789.top/gtdpxsurzh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtxmhitezf.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gtagegmemf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.52xcode.cn/gtxppdfdoj.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtsjtjdlwx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtvwnaziqk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.c1oappe.top/gtmxyjvvfb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtqgsxwdsu.html

[Q47] 与平均值比较
来源：http://hz.ehwqpu.com/gtmvwlceht.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhaomingkeji.xyz/gtfqwaoryt.html

[Q48] CTE 公用表表达式
来源：http://hz.xziqi.cn/gtqggqaezk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydzc1.top/gtuhhzvkwn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cashguo.top/gtilsnutmw.html

[Q49] 更新单行
来源：http://hz.52xcode.cn/gtttisgjip.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtedoqkwfl.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gthyzeythm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nwbrower.top/gtjmrknrvb.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtkmdgigde.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhiwuduotai.top/gtossbawfc.html

[Q52] 删除指定行
来源：http://hz.ivvv.top/gtoxvkzhbe.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtrcmnrcdl.html

[Q53] 按条件删除
来源：http://hz.chenjidiqi.icu/gtjtvmlvgc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dashuyun.cn/gtorlsdrbh.html

[Q54] 清空表
来源：http://hz.hnqzz.top/gtiiorfcsq.html

TRUNCATE TABLE logs;
来源：http://hz.xziqi.cn/gtpugntmzs.html

[Q55] 排名（并列占位）
来源：http://hz.sxryk.cn/gtejzisyps.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gththdytxb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gtelwgxdzc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jlsjyb.cn/gtovlyvocc.html

[Q57] 行号
来源：http://hz.zhoulong.xyz/gteuquubob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigfzy.top/gtjwqtsqil.html

[Q58] 累计求和
来源：http://hz.shzxlz.cn/gtafovodan.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj202588.top/gtfkbrxwny.html

[Q59] 分组内累计
来源：http://hz.zhengqikj.top/gtbyjbklqe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gogol.net.cn/gtnaadklvi.html

[Q60] 取上一行 / 下一行
来源：http://hz.feifeiyinyue.top/gtopasndet.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yanxiufei.cn/gtxpwaqemk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hfpthk.cn/gtszftchnf.html

[Q61] 移动平均
来源：http://hz.cdnleiting.top/gtgegibbqv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daria6918.cn/gtlqdxlxll.html

[Q62] 分组占比
来源：http://hz.hongshengwenyu.top/gtidfewmcb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtxfizdlut.html

[Q63] 开启事务
来源：http://hz.nanxuanxn.top/gtzfljcwdh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xylfe.cn/gtdyvkalgk.html

[Q64] 提交事务
来源：http://hz.bjfxy.top/gtyixvafqj.html

COMMIT;
来源：http://hz.hysaishi.cn/gtfccbnmdz.html

[Q65] 回滚事务
来源：http://hz.ybcxt.top/gtcmgixesz.html

ROLLBACK;
来源：http://hz.tianlin.xyz/gtvsezgmay.html

[Q66] 行锁查询
来源：http://hz.ybcxt.top/gtxvdeqgpy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hongshengwenyu.top/gtishlhspg.html

[Q67] 设置隔离级别
来源：http://hz.nwbrower.top/gtadkceost.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guannengcc.top/gtsswaaygm.html

[Q68] 保存点
来源：http://hz.dashuyun.cn/gtjveexkxo.html

SAVEPOINT sp1;
来源：http://hz.yonumen.top/gtrradzhny.html

ROLLBACK TO sp1;
来源：http://hz.xuanzx.com/gtwylkeifi.html

[Q69] 查看执行计划
来源：http://hz.xylfe.cn/gtxwwcmcyh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhaomingkeji.xyz/gtupgdlpfa.html

[Q70] 更新统计信息
来源：http://hz.zhixingplan.top/gtuexlufmx.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtoungyesc.html

[Q71] 查看建表语句
来源：http://hz.feifeiyinyue.top/gtfewuettj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cqqwz.cn/gtvzlewraj.html

[Q72] 查看索引
来源：http://hz.hfpthk.cn/gtevfieyzv.html

SHOW INDEX FROM users;
来源：http://hz.jinqigufen.top/gtdanebmjd.html

[Q73] 查看表状态
来源：http://hz.fengsongda.top/gtiatqkarr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tanke756.top/gtelgerkzz.html

[Q74] 强制使用索引
来源：http://hz.gzhubu.top/gtuacryekh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhengqikj.top/gtqsmihqzc.html

[Q75] 日期格式化
来源：http://hz.nanxinkj.top/gtxpafmtgj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtppzunoop.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.daria6918.cn/gtwsstrhmo.html

[Q76] 按天统计
来源：http://hz.tanke756.top/gtkkoswook.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtvarjnuib.html

[Q77] 时间加减
来源：http://hz.daxiang520.top/gtqxsopuyl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shzxlz.cn/gtopruhsjj.html

[Q78] 当前时间
来源：http://hz.ydjk.org.cn/gthwvbipiz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuxming.cn/gtpblcplwo.html

[Q79] 字符串拼接
来源：http://hz.hongshengwenyu.top/gtshibtiky.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pengpengdd.cyou/gtyenuzdul.html

[Q80] 字符串截取
来源：http://hz.haohaochexian.top/gtgmdqjncl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtvafjzane.html

[Q81] 字符串替换
来源：http://hz.hfpthk.cn/gtnshriuud.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gtpqksvafu.html

[Q82] 字符长度与字节长度
来源：http://hz.shuidangran.top/gtdxmuvomi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gttadrbxue.html

[Q83] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtshxddryk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtpjhdvztt.html

[Q84] 去除首尾空格
来源：http://hz.wangshuangyany.cn/gtgamhzzen.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigfzy.top/gthttjvxcf.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtymwjugon.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sysykeji.top/gtmdzefcsg.html

[Q86] 读取 JSON 字段
来源：http://hz.chenzaomai.com/gtibupkbvs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtffikjjga.html

[Q87] JSON 字段做条件
来源：http://hz.cucudq.cn/gtrfxcyeys.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jiagoushi.top/gtjfoahxgh.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangdashe.top/gtpfkykpia.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.havefunace.top/gtpjbgzjlk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cashguo.top/gtyqhlwale.html

[Q89] 判断表是否存在
来源：http://hz.ywan-chungtsiang.top/gtwwgcihkr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigfzy.top/gtvrewuthz.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtzlzheypn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydzc1.top/gtrucjkzbb.html

================================================================================
来源：http://hz.zhixingplan.top/gtlhbkjwjs.html

R. Bash 专题
来源：http://hz.jinqigufen.top/gtffnnylrz.html

================================================================================
来源：http://hz.sysykeji.top/gtbpjsmafd.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gttyjrdufm.html

#!/usr/bin/env bash
来源：http://hz.zycfv.cn/gtouxquhym.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtjoazjjfu.html

[R02] 变量赋值与使用
来源：http://hz.yuxming.cn/gtmjmynbfm.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gtkyghjwxf.html

[R03] 只读变量
来源：http://hz.xuanzx.com/gteouujcxs.html

readonly PI=3.14
来源：http://hz.vqdsnc.cn/gtkusmhnqu.html

[R04] 位置参数
来源：http://hz.jianghu66.top/gtdyrgltbi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinghuilouyu.cn/gtbxcfvryb.html

[R05] 参数默认值
来源：http://hz.xziqi.cn/gtkqqvuppf.html

name="${1:-default}"
来源：http://hz.aizwys.cn/gtefgbxink.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gtlmaheqay.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hfpthk.cn/gtvxusqwqt.html

[R07] if 判断文件
来源：http://hz.smart0.xyz/gtakxcnsdp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xylfe.cn/gtltfrseak.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtqkigqzul.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.0kj1m.cn/gtxsqrlxye.html

[R09] 字符串比较
来源：http://hz.dianchejie.cn/gtaampqnya.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtffcpdmiu.html

[R10] 正则匹配
来源：http://hz.9152youxi.cn/gtzcxhsvgf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shzxlz.cn/gtdugztpre.html

[R11] case 多分支
来源：http://hz.nanxinkj.top/gtbmsiahjr.html

case "$1" in
来源：http://hz.ybcxt.top/gtmwnjqmpe.html

start) echo "启动" ;;
来源：http://hz.svipenyu.cn/gthwdxrimr.html

stop)  echo "停止" ;;
来源：http://hz.sxryk.cn/gtidmgpqnv.html

*)     echo "未知命令" ;;
来源：http://hz.hywenlv.cn/gtcmoohywx.html

esac
来源：http://hz.xuanzx.com/gtuuqmxgtg.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtvdbbddoj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgfzy.top/gtntctfxcg.html

[R13] for 计数循环
来源：http://hz.nanxinkj.top/gtgfhahevf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.smart0.xyz/gtpipoeltr.html

[R14] C 风格 for
来源：http://hz.jianghu66.top/gtfcwexxpm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zycfv.cn/gtwttevkbq.html

[R15] while 逐行读文件
来源：http://hz.ydjk.org.cn/gtyemtydty.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhijiandao.cn/gtfqdmixih.html

[R16] until 等待条件
来源：http://hz.c1oappe.top/gtzlybpprf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtzxrxwkgu.html

[R17] 数组定义与取值
来源：http://hz.gzhubu.top/gthdwarfvp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gzhubu.top/gthpymkxdw.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtinxfltyc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtjwlqehep.html

[R19] 数组长度
来源：http://hz.quarkkingdee.top/gtzxkrfoaw.html

echo "${#arr[@]}"
来源：http://hz.nwbrower.top/gtdfzeifgu.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gtoryakqmn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gtjozhrmot.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtlnpuiseb.html

echo "${#s}"
来源：http://hz.yanxiufei.cn/gtrukcixvf.html

[R22] 截取子串
来源：http://hz.9152youxi.cn/gtytyrlbzs.html

echo "${s:0:5}"
来源：http://hz.yuxming.cn/gtdvnqvvai.html

[R23] 字符串替换
来源：http://hz.nanxinkj.top/gtrlovmcdx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xziqi.cn/gtmgllghiv.html

[R24] 大小写转换
来源：http://hz.chenjidiqi.icu/gtkxmgiqui.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gthvlqucyb.html

[R25] 去后缀 / 去前缀
来源：http://hz.kuanghao11.cn/gtcwpbiofa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtodlllirs.html

[R26] 命令替换
来源：http://hz.bjfxy.top/gthexahxna.html

now=$(date +%F); echo "$now"
来源：http://hz.smart0.xyz/gtttwprnqz.html

[R27] 算术展开
来源：http://hz.snrcjt.cn/gtabfapcop.html

echo $((1 + 2 * 3))
来源：http://hz.ehwqpu.com/gtgehengft.html

[R28] 浮点运算
来源：http://hz.wangdashe.top/gtsdejneux.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtohtifmwg.html

[R29] 定义函数
来源：http://hz.yueranfly.top/gtnrlzprok.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xingfuxueyuan.xyz/gttlqqamsm.html

[R30] 函数返回状态码
来源：http://hz.c1oappe.top/gtcqjvoxue.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cdnleiting.top/gtaxvxzbhc.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gtpepxucra.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenjidiqi.icu/gtynklzngw.html

[R32] 参数个数校验
来源：http://hz.ehwqpu.com/gtgvklnohn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xylfe.cn/gtktuenqxn.html

[R33] 捕获错误并提示行号
来源：http://hz.guannengcc.top/gtnxldzrqp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ywan-chungtsiang.top/gtthpuarsr.html

[R34] 退出时清理
来源：http://hz.hnxiangtu.top/gtqnkleadq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtfcanhvkx.html

[R35] 后台执行并等待
来源：http://hz.cheryme.top/gtewwuzqeq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtybdqkwdl.html

[R36] 并发执行多个任务
来源：http://hz.xinyue.icu/gtbaplribv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gaohongyu789.top/gtpkpskssd.html

[R37] 把输出赋给变量
来源：http://hz.birdmap.top/gtlwjmiokv.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtvlrwetbu.html

[R38] 管道串联
来源：http://hz.xziqi.cn/gtkahfpsis.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtxkglhyhl.html

[R39] 重定向标准输出与错误
来源：http://hz.yj202588.top/gtxvnatdng.html

cmd > out.log 2>&1
来源：http://hz.daxiang520.top/gtjqnuqobx.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtmfffrwqn.html

echo "log" >> out.log
来源：http://hz.sysykeji.top/gtiojavkrt.html

[R41] 丢弃输出
来源：http://hz.wangshuangyany.cn/gtgawwxelx.html

cmd >/dev/null 2>&1
来源：http://hz.aizwys.cn/gtsljviaqx.html

[R42] 输入重定向
来源：http://hz.daxiang520.top/gtbyvifppk.html

wc -l < a.txt
来源：http://hz.cheryme.top/gtpkjbcfkd.html

[R43] 按名字查找文件
来源：http://hz.xinyue.icu/gtnsymoeum.html

find . -name "*.log" -type f
来源：http://hz.daria6918.cn/gtuaagntck.html

[R44] 按修改时间查找
来源：http://hz.wangdashe.top/gtscibenrf.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtwaekszky.html

[R45] 批量删除
来源：http://hz.jinghuilouyu.cn/gtllhavaut.html

find . -name "*.tmp" -delete
来源：http://hz.52xcode.cn/gtcrlhskuc.html

[R46] 递归替换文件内容
来源：http://hz.quarkkingdee.top/gtacmudiou.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zdqjudy.top/gtzeijiyyz.html

[R47] sed 单行替换
来源：http://hz.snrcjt.cn/gttleaqsmi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuxming.cn/gtwcuzgrty.html

[R48] awk 取指定列
来源：http://hz.zhaomingkeji.xyz/gtgkrhiolz.html

awk '{print $1, $3}' a.txt
来源：http://hz.daxiang520.top/gtaplnejnn.html

[R49] awk 带条件
来源：http://hz.pycfn.com/gtdemtfqzo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangkeji.top/gtluqqqbjb.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtjdphsbex.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tianlin.xyz/gtullaepwf.html

[R51] 排序去重取前几
来源：http://hz.ydzc1.top/gtwhtmspuj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tian-w.cn/gtdfkotmwz.html

[R52] 统计行数
来源：http://hz.dianchejie.cn/gtzlypyjkz.html

wc -l a.txt
来源：http://hz.tanke756.top/gtamdruill.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtekihxvau.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gogol.net.cn/gtlhzybvyd.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtbpekwdjb.html

diff a.txt b.txt
来源：http://hz.yangfankeji.com/gtewtbziyc.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gtzdmsuhby.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtfvnfvhvm.html

[R56] 远程拷贝
来源：http://hz.yueranfly.top/gtkkyyndqf.html

scp file user@host:/path/
来源：http://hz.zhengqikj.top/gtmikqrcys.html

[R57] 远程执行命令
来源：http://hz.ydzc1.top/gthbzvqrlm.html

ssh user@host 'uptime'
来源：http://hz.jlsjyb.cn/gteumdvgzj.html

[R58] 下载文件
来源：http://hz.gaohongyu789.top/gtcwzbahxt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sysykeji.top/gtqfiklivy.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gtqzrtkwvx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangshuangyany.cn/gtlpydgcfl.html

[R60] 只看 HTTP 状态码
来源：http://hz.zdqjudy.top/gtaonuqlje.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhoulong.xyz/gtwlweduhp.html

[R61] 磁盘占用
来源：http://hz.birdmap.top/gtrluwozdd.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gttftlkpqk.html

[R62] 找最占空间的文件
来源：http://hz.jinqigfzy.top/gtoarolibg.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtoqnjjcfu.html

[R63] 内存与进程
来源：http://hz.jinqigufen.top/gtedrubmek.html

free -h;  ps aux | grep nginx
来源：http://hz.yangfankeji.com/gtxscbxvvi.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtaxgvsifm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yonumen.top/gtxcpwdyhc.html

[R65] 查看端口占用
来源：http://hz.yj20258888.top/gtotwlhkwu.html


<!-- 参考信息 -->