代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtlobohlpv.html

[Q28] 求和与平均
来源：http://hz.zdqjudy.top/gtyujrxzui.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gtvfomdslp.html

[Q29] 最大最小值
来源：http://hz.yj202588.top/gtlghhpfum.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pengpengdd.cyou/gtjgnlgvqj.html

[Q30] 分组统计
来源：http://hz.0kj1m.cn/gtugrjmuzn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gttzyfvvgo.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtbphegvbl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yongpay.top/gthimvlkbz.html

[Q32] 分组拼接字符串
来源：http://hz.wangdashe.top/gtodqoxypu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtpfvyxdui.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangshuangyany.cn/gtkvphucuj.html

[Q33] 多列分组
来源：http://hz.tianlin.xyz/gtfiewnyzc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinghuilouyu.cn/gtyfwosjac.html

[Q34] 每组取第一条
来源：http://hz.sufxvd.cn/gtnoxujkfc.html

SELECT * FROM (
来源：http://hz.zhaomingkeji.xyz/gtxvzvlbht.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ppjwa.cn/gtnkfvozbd.html

) t WHERE rn = 1;
来源：http://hz.yvedp.cn/gtwsjmdpbg.html

[Q35] 内连接
来源：http://hz.jianghu66.top/gtjdajqeja.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtfhcsflil.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtqgbhrfpw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtmieixzbe.html

[Q37] 右连接
来源：http://hz.yongpay.top/gtwtcubwsj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guowangkeji.top/gtltbjkcqm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cashguo.top/gtyicjarhn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ivvv.top/gtnwyywhpq.html

[Q39] 自连接（查上下级）
来源：http://hz.cashguo.top/gtoojghuae.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yonumen.top/gtklmhbcgd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ehwqpu.com/gtzcyrartj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.iojbl.cn/gtgxehcckg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhongyouzk.top/gtebivvbuk.html

[Q41] 多表连接
来源：http://hz.aibaodan.cn/gtzdaropkb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtydgaesbx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.dianchejie.cn/gtvnhjyouu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yanxiufei.cn/gtnistpqef.html

[Q42] 连接条件附加过滤
来源：http://hz.cqqwz.cn/gtlcdolhvg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.c1oappe.top/gtkeezyxue.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ywan-chungtsiang.top/gtzalgjvif.html

[Q43] 标量子查询
来源：http://hz.ivvv.top/gtpdycmakx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhiwuduotai.top/gtgurukiwy.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gtjdvyqzid.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.52xcode.cn/gtqcgpdqaz.html

[Q45] EXISTS 判断存在
来源：http://hz.zhijiandao.cn/gtsupdgjnq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtkylhyffi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hfpthk.cn/gtsbximpol.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtoskqxafo.html

[Q47] 与平均值比较
来源：http://hz.yvedp.cn/gtfxqjzdry.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gtfagkrolt.html

[Q48] CTE 公用表表达式
来源：http://hz.nwbrower.top/gtnclvorct.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sufxvd.cn/gtctatjkap.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtwpjhtghy.html

[Q49] 更新单行
来源：http://hz.chenjidiqi.icu/gtvlxalsfm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dashuyun.cn/gtazqhaovl.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtpvkhelmt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenzaomai.com/gtfyfepevz.html

[Q51] 用子查询更新
来源：http://hz.yangfankeji.com/gtencbskey.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhongyouzk.top/gtbdibgzoc.html

[Q52] 删除指定行
来源：http://hz.gaohongyu789.top/gtugciytol.html

DELETE FROM users WHERE id = 10;
来源：http://hz.snrcjt.cn/gthyzpzpoj.html

[Q53] 按条件删除
来源：http://hz.bjfxy.top/gtywpysino.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hysaishi.cn/gtwcvtjjse.html

[Q54] 清空表
来源：http://hz.bjfxy.top/gtprwcrlij.html

TRUNCATE TABLE logs;
来源：http://hz.xingfuxueyuan.xyz/gtesroueru.html

[Q55] 排名（并列占位）
来源：http://hz.shangyingyoupin.top/gtdoidwcoq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydjk.org.cn/gtehesmryo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.vqdsnc.cn/gtfhsjofyp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangshuangyany.cn/gtyqqeuchv.html

[Q57] 行号
来源：http://hz.jyoumei.cn/gtuojsktck.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgufenzy.top/gthhxtacac.html

[Q58] 累计求和
来源：http://hz.jinyuanbaomall.cn/gtvgbmaxru.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sufxvd.cn/gtsxqzoszu.html

[Q59] 分组内累计
来源：http://hz.haohaochexian.top/gtghkbscgl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtuwymsweu.html

[Q60] 取上一行 / 下一行
来源：http://hz.316326.xyz/gtqiwnnsxw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtbqurlwwh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ivvv.top/gtlgmmlwse.html

[Q61] 移动平均
来源：http://hz.sxryk.cn/gtuszowbwi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tianlin.xyz/gtsrjpobzl.html

[Q62] 分组占比
来源：http://hz.hysaishi.cn/gtvsevvyhl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtsqobhfrf.html

[Q63] 开启事务
来源：http://hz.yonumen.top/gtprwrgbim.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tanke756.top/gtodapeqtf.html

[Q64] 提交事务
来源：http://hz.xylfe.cn/gtssznkrtl.html

COMMIT;
来源：http://hz.xuanzx.com/gtpqevcqiu.html

[Q65] 回滚事务
来源：http://hz.haohaochexian.top/gtkomrtrwl.html

ROLLBACK;
来源：http://hz.meibo888.top/gtomsjixqg.html

[Q66] 行锁查询
来源：http://hz.redwolf501.top/gtmxjazflz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtimvjbeax.html

[Q67] 设置隔离级别
来源：http://hz.yj20258.top/gtncnupqrx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangshuangyany.cn/gtzhpjapra.html

[Q68] 保存点
来源：http://hz.cashguo.top/gtvsunvqpp.html

SAVEPOINT sp1;
来源：http://hz.sweek.top/gtxkerjfvu.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gttmqoyfbk.html

[Q69] 查看执行计划
来源：http://hz.haohaochexian.top/gtpxauhugt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxinkj.top/gtrxgehuqi.html

[Q70] 更新统计信息
来源：http://hz.guannengcc.top/gtebbqhllv.html

ANALYZE TABLE users;
来源：http://hz.mhx1999.top/gtodxjtdks.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtixplkwil.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtzvxbxmrj.html

[Q72] 查看索引
来源：http://hz.gzhubu.top/gtxyyoiimk.html

SHOW INDEX FROM users;
来源：http://hz.haohaochexian.top/gtfleneany.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtyrrrxlbp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fzhhl.top/gtwsmliata.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtvxfhlpdm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuetiantiany.cn/gtvtczpkya.html

[Q75] 日期格式化
来源：http://hz.vqdsnc.cn/gteyzzseww.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tian-w.cn/gtdueppljk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cqqwz.cn/gtjdnttlvf.html

[Q76] 按天统计
来源：http://hz.ydjk.org.cn/gtlnzixhtq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tanke756.top/gtfhyowpzv.html

[Q77] 时间加减
来源：http://hz.jinqigfzy.top/gtkmdesela.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.feifeiyinyue.top/gtrdbwcqhz.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtfotqmvqh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dashuyun.cn/gtrhspjpth.html

[Q79] 字符串拼接
来源：http://hz.dianchejie.cn/gtmrqbhsti.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cucudq.cn/gtklxlxite.html

[Q80] 字符串截取
来源：http://hz.shangyingyoupin.top/gtzoneesni.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.mhx1999.top/gtkqmfxnkh.html

[Q81] 字符串替换
来源：http://hz.chenlongwang.top/gtwdwzbdkv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxuanxn.top/gtycjronll.html

[Q82] 字符长度与字节长度
来源：http://hz.ppjwa.cn/gtulcpbcqk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cucudq.cn/gtyjjfhnfo.html

[Q83] 大小写转换
来源：http://hz.havefunace.top/gtofwlektm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.vqdsnc.cn/gtzgvuegfj.html

[Q84] 去除首尾空格
来源：http://hz.tianlin.xyz/gtqlhamtkk.html

SELECT TRIM(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtzilgklac.html

[Q85] 数值取整
来源：http://hz.cdnleiting.top/gtfcbmjjsw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenjidiqi.icu/gtsvruypkn.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gtyovaszgk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigfzy.top/gtfwsezxqh.html

[Q87] JSON 字段做条件
来源：http://hz.zhixingplan.top/gtczcdibzc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgufenzy.top/gtxrvxjibu.html

[Q88] 行转列（条件聚合）
来源：http://hz.ehwqpu.com/gtckctbskt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.haohaochexian.top/gtmxtxboxs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.9152youxi.cn/gtjyttzwph.html

[Q89] 判断表是否存在
来源：http://hz.guowangkeji.top/gtmqlwwggl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hfpthk.cn/gtfzjdnebg.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtppquetgl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtdjwfjqbp.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtseflzuha.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtlbmslgvn.html

================================================================================
来源：http://hz.yj20258888.top/gtegpyocnr.html

[R01] shebang 与严格模式
来源：http://hz.guowangkeji.top/gtshslvvzg.html

#!/usr/bin/env bash
来源：http://hz.9152youxi.cn/gtfykpmusg.html

set -euo pipefail
来源：http://hz.nwbrower.top/gthemapabt.html

[R02] 变量赋值与使用
来源：http://hz.xziqi.cn/gturhfsspd.html

name="Tom"; echo "$name"
来源：http://hz.fengsongda.top/gtajgzgozf.html

[R03] 只读变量
来源：http://hz.ywan-chungtsiang.top/gtmyslzpya.html

readonly PI=3.14
来源：http://hz.316326.xyz/gtifwprdgn.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gttjbxqyqx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jyoumei.cn/gtwzxikkft.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtuawiaeys.html

name="${1:-default}"
来源：http://hz.haohaochexian.top/gteontqgxh.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gtrrokdbyh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tianlin.xyz/gtbbhlumpl.html

[R07] if 判断文件
来源：http://hz.nwbrower.top/gtpaydhxwd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.svipenyu.cn/gtuhfcobpj.html

[R08] 数值比较
来源：http://hz.hnxiangtu.top/gtgmnplnwc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenlongwang.top/gtevvhndrr.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gthlgqfoxy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.guowangkeji.top/gtwqnucnxw.html

[R10] 正则匹配
来源：http://hz.guowangkeji.top/gtlqhzcevz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.vqdsnc.cn/gthzeujsid.html

[R11] case 多分支
来源：http://hz.xziqi.cn/gtiobgankf.html

case "$1" in
来源：http://hz.xingfuxueyuan.xyz/gtnbppifbz.html

start) echo "启动" ;;
来源：http://hz.shzxlz.cn/gthmfprdtf.html

stop)  echo "停止" ;;
来源：http://hz.yueranfly.top/gtthahsspe.html

*)     echo "未知命令" ;;
来源：http://hz.haohaochexian.top/gthxwgsmgd.html

esac
来源：http://hz.cashguo.top/gtkqgwspds.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gtubiotbsj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhixingplan.top/gtefyjxtgh.html

[R13] for 计数循环
来源：http://hz.zhijiandao.cn/gtrzhxxueu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shzxlz.cn/gttxtnehaa.html

[R14] C 风格 for
来源：http://hz.ydzc1.top/gtjcetbxec.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtoyjqdctx.html

[R15] while 逐行读文件
来源：http://hz.gzhubu.top/gtvvvsarek.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtidqqbnjv.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gthmkulalc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gtmnjdulwt.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gthcjsixtu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtmjllosit.html

[R18] 遍历数组
来源：http://hz.jianghu66.top/gtnjiptruv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gtkabodnot.html

[R19] 数组长度
来源：http://hz.aibaodan.cn/gtfsfazkpa.html

echo "${#arr[@]}"
来源：http://hz.zhiwuduotai.top/gtuaybyowb.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtwnaujala.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtakviwdvg.html

[R21] 字符串长度
来源：http://hz.guowangkeji.top/gtaamqynrm.html

echo "${#s}"
来源：http://hz.zdqjudy.top/gtgnpibbiz.html

[R22] 截取子串
来源：http://hz.nwbrower.top/gtwpvyeycf.html

echo "${s:0:5}"
来源：http://hz.cheryme.top/gtkepixsjf.html

[R23] 字符串替换
来源：http://hz.xylfe.cn/gtzkijbpyi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ppjwa.cn/gtcxcaifjp.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gtwkarmbra.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhixingplan.top/gtyvdvpdto.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgfzy.top/gtbjepdvfi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtpxmpuwen.html

[R26] 命令替换
来源：http://hz.daria6918.cn/gtrflyxzwn.html

now=$(date +%F); echo "$now"
来源：http://hz.kuanghao11.cn/gtaibdbdyi.html

[R27] 算术展开
来源：http://hz.zhongyouzk.top/gtyuiwbvii.html

echo $((1 + 2 * 3))
来源：http://hz.iojbl.cn/gthqwnobrp.html

[R28] 浮点运算
来源：http://hz.nanxinkj.top/gtueyxbokx.html

echo "scale=2; 10/3" | bc
来源：http://hz.xylfe.cn/gtozhbuaeq.html

[R29] 定义函数
来源：http://hz.nanxinkj.top/gtfiuaoyte.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yvedp.cn/gtzdjrypvl.html

[R30] 函数返回状态码
来源：http://hz.haohaochexian.top/gtzilbzakp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daria6918.cn/gtaklfbbsf.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gtbltzpylx.html

f() { local x=1; echo "$x"; }
来源：http://hz.yonumen.top/gtevaybrwj.html

[R32] 参数个数校验
来源：http://hz.zhijiandao.cn/gtpguppxfz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jlsjyb.cn/gtbmritxff.html

[R33] 捕获错误并提示行号
来源：http://hz.gzhubu.top/gtwtqthfis.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yangfankeji.com/gtwvovrtfx.html

[R34] 退出时清理
来源：http://hz.yj20258888.top/gtyxmjkadp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtsaypoeph.html

[R35] 后台执行并等待
来源：http://hz.ivvv.top/gtbhlwqbqz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shzxlz.cn/gtmjyagspv.html

[R36] 并发执行多个任务
来源：http://hz.ybcxt.top/gtvmwnqpcu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yanxiufei.cn/gtrqxwtnpc.html

[R37] 把输出赋给变量
来源：http://hz.jinqigufen.top/gtrtiammye.html

files=$(ls -1)
来源：http://hz.fzhhl.top/gtnswdlmgt.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtfiybgpvx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhoulong.xyz/gtjovsmrwy.html

[R39] 重定向标准输出与错误
来源：http://hz.c1oappe.top/gtwaryteoy.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtrktwcicv.html

[R40] 追加写日志
来源：http://hz.jinghuilouyu.cn/gtcdkykoch.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gtnzmdvthz.html

[R41] 丢弃输出
来源：http://hz.tianlin.xyz/gtnfnbwefn.html

cmd >/dev/null 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtrjgycwke.html

[R42] 输入重定向
来源：http://hz.havefunace.top/gtnmhizfpl.html

wc -l < a.txt
来源：http://hz.aizwys.cn/gttwsaifse.html

[R43] 按名字查找文件
来源：http://hz.0kj1m.cn/gtgsohdjcp.html

find . -name "*.log" -type f
来源：http://hz.fzhhl.top/gtxhdsqzih.html

[R44] 按修改时间查找
来源：http://hz.kuanghao11.cn/gtphcirvzm.html

find . -mtime -7 -type f
来源：http://hz.nwbrower.top/gtzlmjlgcu.html

[R45] 批量删除
来源：http://hz.yj202588.top/gtzpazhgoa.html

find . -name "*.tmp" -delete
来源：http://hz.sxryk.cn/gtaelketui.html

[R46] 递归替换文件内容
来源：http://hz.hnqzz.top/gtvtdprdej.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.dashuyun.cn/gtcosvbnkt.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtxoxdfzde.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.316326.xyz/gtckqrrxkm.html

[R48] awk 取指定列
来源：http://hz.hammf.cn/gtyqycccnm.html

awk '{print $1, $3}' a.txt
来源：http://hz.xziqi.cn/gtgidhdzgi.html

[R49] awk 带条件
来源：http://hz.gzhubu.top/gtuowcxffr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hammf.cn/gtwxjlaurh.html

[R50] awk 求和
来源：http://hz.zhijiandao.cn/gtgmkzadrw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gaohongyu789.top/gtxrwnaleo.html

[R51] 排序去重取前几
来源：http://hz.haohaochexian.top/gtducdopcd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenlongwang.top/gtjgqzxtdk.html

[R52] 统计行数
来源：http://hz.meibo888.top/gtziaaeytq.html

wc -l a.txt
来源：http://hz.zhengqikj.top/gtixvrhrup.html

[R53] 查看文件头与实时尾
来源：http://hz.yuanzhike.top/gtytlpllgm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.vqdsnc.cn/gthuvgtvgl.html

[R54] 比较两个文件
来源：http://hz.daria6918.cn/gtvjwilwri.html

diff a.txt b.txt
来源：http://hz.wangshuangyany.cn/gtyirophcz.html

[R55] 压缩与解压
来源：http://hz.smart0.xyz/gtnnmfzpfd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtseydkeah.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gtfitobocl.html

scp file user@host:/path/
来源：http://hz.ydjk.org.cn/gtadwagoos.html

[R57] 远程执行命令
来源：http://hz.yvedp.cn/gtlrktupev.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gtdpmpqcuy.html

[R58] 下载文件
来源：http://hz.svipenyu.cn/gtakqocjpu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nwbrower.top/gtsuuqafro.html

[R59] 发 POST JSON
来源：http://hz.hywenlv.cn/gtxspcpzdj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yanxiufei.cn/gtjyzodmec.html

[R60] 只看 HTTP 状态码
来源：http://hz.yueranfly.top/gtkjuhcysm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigufen.top/gtihtwuucr.html

[R61] 磁盘占用
来源：http://hz.ppjwa.cn/gtsdqxqcmw.html

df -h;  du -sh *
来源：http://hz.yongpay.top/gtmovyirlb.html

[R62] 找最占空间的文件
来源：http://hz.sxryk.cn/gturlfaxfy.html

du -ah . | sort -rh | head -10
来源：http://hz.gogol.net.cn/gtvkgjcdks.html

[R63] 内存与进程
来源：http://hz.zhijiandao.cn/gtdjmpkgsh.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgfzy.top/gtzczutqus.html

[R64] 结束进程
来源：http://hz.316326.xyz/gtgcsgelzo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangtech.top/gtlanznnia.html

[R65] 查看端口占用
来源：http://hz.0kj1m.cn/gtamtflyga.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtuoolfxjz.html

[R66] 定时任务
来源：http://hz.aizwys.cn/gtzicbjues.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gtoqznnduz.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtqajgboco.html

openssl rand -hex 16
来源：http://hz.cucudq.cn/gthaehflaj.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangtech.top/gtwwzhmidl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhijiandao.cn/gttwdemces.html

[R69] 生成随机密码
来源：http://hz.ybcxt.top/gtiohkupkb.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenlongwang.top/gtkdnignmr.html

[R70] 时间戳与互转
来源：http://hz.jqgfzy.top/gtbenrxcjc.html

date +%s;  date -d @1700000000
来源：http://hz.yonumen.top/gtnnfxqpwq.html

[R71] 日期格式化
来源：http://hz.yj20258.top/gtothkvrjm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ivvv.top/gtsrvwglfw.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gtsebbgyth.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenlongwang.top/gtyatssvhf.html

[R73] 分割大日志
来源：http://hz.sufxvd.cn/gttxreexir.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gttcubpzew.html

[R74] 批量重命名
来源：http://hz.yj20258.top/gtulhszxww.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hongshengwenyu.top/gtrxlghazm.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtasrqsovm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.havefunace.top/gtozivgmby.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtaigeihar.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtucmjzlwf.html

[R77] 读取用户输入
来源：http://hz.yonumen.top/gtrwekkkxp.html


<!-- 参考信息 -->