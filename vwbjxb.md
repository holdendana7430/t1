代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hz.hysaishi.cn/gtuwrcnkko.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hywenlv.cn/gteurzislo.html

[Q43] 标量子查询
来源：http://hz.jlsjyb.cn/gtayzlndol.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hongshengwenyu.top/gtiseztdim.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangkeji.top/gtjpybfeuu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tianlin.xyz/gtgyealmkb.html

[Q45] EXISTS 判断存在
来源：http://hz.fengsongda.top/gtkifbcqai.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtmcplxrsl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.daxiang520.top/gtvqjjjnwv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydzc1.top/gtofmvmamk.html

[Q47] 与平均值比较
来源：http://hz.wangshuangyany.cn/gtwottznas.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenlongwang.top/gtqzakgemg.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtxnlbhxqu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cucudq.cn/gtyksocdfy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jlsjyb.cn/gtvxyxseaf.html

[Q49] 更新单行
来源：http://hz.yvedp.cn/gtnllsqqwd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gtulxbbssj.html

[Q50] 批量更新
来源：http://hz.yj20258.top/gtsjsoztug.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cashguo.top/gtlulljzvh.html

[Q51] 用子查询更新
来源：http://hz.bjfxy.top/gtscxytbzr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigufen.top/gtwufkdcnk.html

[Q52] 删除指定行
来源：http://hz.zhixingplan.top/gtothezsdz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.havefunace.top/gtybfmxukk.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtpajdspva.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sufxvd.cn/gteatylogz.html

[Q54] 清空表
来源：http://hz.52xcode.cn/gtqysbkakc.html

TRUNCATE TABLE logs;
来源：http://hz.ivvv.top/gtrbzvgaxq.html

[Q55] 排名（并列占位）
来源：http://hz.xylfe.cn/gtcwjlyhnj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.fengsongda.top/gtsmlkdkty.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cqqwz.cn/gtjgfcywsh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.snrcjt.cn/gtxmutynqx.html

[Q57] 行号
来源：http://hz.sysykeji.top/gtflltuvda.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aizwys.cn/gtuxdyhfuq.html

[Q58] 累计求和
来源：http://hz.jqgfzy.top/gtzwijgdmc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtkuixcwjm.html

[Q59] 分组内累计
来源：http://hz.guannengcc.top/gtsttvddqj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.andypj.xyz/gtapydkehb.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gtowvgjyda.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtjrwdjjae.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.mhx1999.top/gttvljsgwz.html

[Q61] 移动平均
来源：http://hz.yongpay.top/gtdsrltdnw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dianchejie.cn/gticwkimnm.html

[Q62] 分组占比
来源：http://hz.yanxiufei.cn/gtfckgpyzv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtpuugjcvc.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gtuegblhnt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hammf.cn/gttezeilvx.html

[Q64] 提交事务
来源：http://hz.ppjwa.cn/gtrtdkeywp.html

COMMIT;
来源：http://hz.snrcjt.cn/gtofwxpntr.html

[Q65] 回滚事务
来源：http://hz.svipenyu.cn/gtcsnmavzd.html

ROLLBACK;
来源：http://hz.yangfankeji.com/gthawpjjef.html

[Q66] 行锁查询
来源：http://hz.ywan-chungtsiang.top/gtwndfoekk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tanke756.top/gttnkddbid.html

[Q67] 设置隔离级别
来源：http://hz.yj20258888.top/gtuxhctaas.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinghuilouyu.cn/gtkkrxxzms.html

[Q68] 保存点
来源：http://hz.yvedp.cn/gtaqycenkc.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtfuakxffp.html

ROLLBACK TO sp1;
来源：http://hz.daxiang520.top/gtfiaomtpt.html

[Q69] 查看执行计划
来源：http://hz.yongpay.top/gtfynljuei.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtxqqkfcxs.html

[Q70] 更新统计信息
来源：http://hz.dashuyun.cn/gtstdfpldg.html

ANALYZE TABLE users;
来源：http://hz.guannengcc.top/gtcjjrnjls.html

[Q71] 查看建表语句
来源：http://hz.feifeiyinyue.top/gtuvgslmup.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gtuxjuujwq.html

[Q72] 查看索引
来源：http://hz.jinyuanbaomall.cn/gtqqbxrfac.html

SHOW INDEX FROM users;
来源：http://hz.yanxiufei.cn/gtahhxtkpa.html

[Q73] 查看表状态
来源：http://hz.sufxvd.cn/gtrqvzjatc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.bjfxy.top/gtquyfvlzd.html

[Q74] 强制使用索引
来源：http://hz.hywenlv.cn/gtqsbmduns.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hongshengwenyu.top/gtbdhjbgfo.html

[Q75] 日期格式化
来源：http://hz.sufxvd.cn/gtodqlbgwh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinghuilouyu.cn/gtiiyfavka.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gthftdeszp.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtnsghpgul.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.birdmap.top/gtqauvbkyf.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtixylgrin.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtsclvdfam.html

[Q78] 当前时间
来源：http://hz.hywenlv.cn/gtbhrzycbn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gtwyfjrkbn.html

[Q79] 字符串拼接
来源：http://hz.pengpengdd.cyou/gtqvdkepqa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.vqdsnc.cn/gtmghuuita.html

[Q80] 字符串截取
来源：http://hz.shangyingyoupin.top/gttlvmcknq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtyqmbfkvo.html

[Q81] 字符串替换
来源：http://hz.bjfxy.top/gtvkqwmzbw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxinkj.top/gtvukwasbj.html

[Q82] 字符长度与字节长度
来源：http://hz.haohaochexian.top/gtqnnjtbjf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shzxlz.cn/gtzedzknds.html

[Q83] 大小写转换
来源：http://hz.xziqi.cn/gttecxpkow.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fzhhl.top/gttkarmwqc.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangkeji.top/gtnusjiiep.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtdafpskzd.html

[Q85] 数值取整
来源：http://hz.vqdsnc.cn/gtsebtogjj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtckjojpbz.html

[Q86] 读取 JSON 字段
来源：http://hz.shuidangran.top/gtjyxiocor.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ehwqpu.com/gtrthtexux.html

[Q87] JSON 字段做条件
来源：http://hz.xziqi.cn/gtwrqhsryz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cucudq.cn/gtffwushhg.html

[Q88] 行转列（条件聚合）
来源：http://hz.ehwqpu.com/gtbuugbyog.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tanke756.top/gtgkumnmyo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenjidiqi.icu/gtfualqnxq.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtmupkimsn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gttnuhzmpl.html

[Q90] 生成序号列
来源：http://hz.jqgfzy.top/gtaegjqvmj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.quarkkingdee.top/gteaysbnoa.html

================================================================================
来源：http://hz.yuxming.cn/gtplheqlax.html

R. Bash 专题
来源：http://hz.quarkkingdee.top/gthisdmhji.html

================================================================================
来源：http://hz.aibaodan.cn/gtquzxrydq.html

[R01] shebang 与严格模式
来源：http://hz.wangdashe.top/gtattcnepg.html

#!/usr/bin/env bash
来源：http://hz.jinghuilouyu.cn/gtkdccdibl.html

set -euo pipefail
来源：http://hz.feifeiyinyue.top/gtntpztkfh.html

[R02] 变量赋值与使用
来源：http://hz.chenzaomai.com/gtpzqnhexf.html

name="Tom"; echo "$name"
来源：http://hz.yanxiufei.cn/gtikwzjano.html

[R03] 只读变量
来源：http://hz.jiagoushi.top/gtewcytino.html

readonly PI=3.14
来源：http://hz.mhx1999.top/gtouwwjiuw.html

[R04] 位置参数
来源：http://hz.yvedp.cn/gtbkxqzlcu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.aizwys.cn/gtwqkiovza.html

[R05] 参数默认值
来源：http://hz.dashuyun.cn/gtczcfkcgy.html

name="${1:-default}"
来源：http://hz.jqgfzy.top/gtdgkocqwo.html

[R06] 判断命令是否存在
来源：http://hz.zhoulong.xyz/gtougnikgz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.snrcjt.cn/gtyldzkkhj.html

[R07] if 判断文件
来源：http://hz.zdqjudy.top/gtayazfqdj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gttknxliye.html

[R08] 数值比较
来源：http://hz.ybcxt.top/gtnajeeexs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sufxvd.cn/gttydcjnig.html

[R09] 字符串比较
来源：http://hz.xuetiantiany.cn/gtmcvijcre.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zycfv.cn/gtzaiqhvmy.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtbygrvkis.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hammf.cn/gtapcxdfgw.html

[R11] case 多分支
来源：http://hz.jinyuanbaomall.cn/gtievawrvh.html

case "$1" in
来源：http://hz.ydzc1.top/gtilrxkmrt.html

start) echo "启动" ;;
来源：http://hz.hongshengwenyu.top/gtlnxtxaom.html

stop)  echo "停止" ;;
来源：http://hz.ydjk.org.cn/gtosoqttga.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gtreijskwy.html

esac
来源：http://hz.cheryme.top/gtxlopzzsu.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtwbglhfer.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daria6918.cn/gtjucenyxe.html

[R13] for 计数循环
来源：http://hz.9152youxi.cn/gthezqdksi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yvedp.cn/gtzuwichoc.html

[R14] C 风格 for
来源：http://hz.pengpengdd.cyou/gticchqjkq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtrogxzgxh.html

[R15] while 逐行读文件
来源：http://hz.c1oappe.top/gtfnyyrgjt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuetiantiany.cn/gtvukaxpnr.html

[R16] until 等待条件
来源：http://hz.aibaodan.cn/gtmbzjpiuf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xylfe.cn/gtmeynpkds.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gtyhtypyih.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tanke756.top/gtzucoenhr.html

[R18] 遍历数组
来源：http://hz.yonumen.top/gtkcunldlu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgfzy.top/gtgxjgwinl.html

[R19] 数组长度
来源：http://hz.xinyue.icu/gtowraaxtr.html

echo "${#arr[@]}"
来源：http://hz.meibo888.top/gttllxaess.html

[R20] 关联数组（字典）
来源：http://hz.shzxlz.cn/gtlkqxtdik.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zycfv.cn/gtbkilbbba.html

[R21] 字符串长度
来源：http://hz.chenjidiqi.icu/gthnxaatja.html

echo "${#s}"
来源：http://hz.sufxvd.cn/gtrbpozyaz.html

[R22] 截取子串
来源：http://hz.jianghu66.top/gtflbhbpkl.html

echo "${s:0:5}"
来源：http://hz.hnxiangtu.top/gttuggqjvj.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtfkkcmxda.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangkeji.top/gtzeqewdei.html

[R24] 大小写转换
来源：http://hz.tanke756.top/gtszsistoi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xziqi.cn/gtqlmdelbs.html

[R25] 去后缀 / 去前缀
来源：http://hz.pycfn.com/gtipwqspjb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shuidangran.top/gtnrmffrcg.html

[R26] 命令替换
来源：http://hz.aizwys.cn/gtxjemhmse.html

now=$(date +%F); echo "$now"
来源：http://hz.daria6918.cn/gtfwswsdbz.html

[R27] 算术展开
来源：http://hz.hywenlv.cn/gtteuqaglf.html

echo $((1 + 2 * 3))
来源：http://hz.hysaishi.cn/gtgyqmynxl.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gtizeetfql.html

echo "scale=2; 10/3" | bc
来源：http://hz.pengpengdd.cyou/gtdzrmekec.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gticebidxp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtzljqpryl.html

[R30] 函数返回状态码
来源：http://hz.birdmap.top/gttuibsnqf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.0kj1m.cn/gtywbaswjp.html

[R31] 局部变量
来源：http://hz.yonumen.top/gtelisyudr.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigfzy.top/gtuuyhrjba.html

[R32] 参数个数校验
来源：http://hz.ydjk.org.cn/gtpjwohkgf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yangfankeji.com/gtpjadphzc.html

[R33] 捕获错误并提示行号
来源：http://hz.jiagoushi.top/gtdkzvidee.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtklxyfnmm.html

[R34] 退出时清理
来源：http://hz.ppjwa.cn/gtummzzyth.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtpxsslwim.html

[R35] 后台执行并等待
来源：http://hz.nwbrower.top/gteutauimp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ybcxt.top/gtbqqeijjs.html

[R36] 并发执行多个任务
来源：http://hz.zhaomingkeji.xyz/gticxayhzm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtsfdcjrjl.html

[R37] 把输出赋给变量
来源：http://hz.ehwqpu.com/gtlhgrarai.html

files=$(ls -1)
来源：http://hz.nanxuanxn.top/gtbgizzrvj.html

[R38] 管道串联
来源：http://hz.ybcxt.top/gturhftelh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.quarkkingdee.top/gtfbqthfdn.html

[R39] 重定向标准输出与错误
来源：http://hz.guannengcc.top/gtbuzgysxj.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtrlfnsuto.html

[R40] 追加写日志
来源：http://hz.xylfe.cn/gttcgeztyp.html

echo "log" >> out.log
来源：http://hz.ybcxt.top/gtjwzfunru.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtteisnobs.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gtvjgdwbqz.html

[R42] 输入重定向
来源：http://hz.ydzc1.top/gteycnpmjs.html

wc -l < a.txt
来源：http://hz.dianchejie.cn/gtczftvcrw.html

[R43] 按名字查找文件
来源：http://hz.jqgfzy.top/gtajqhlhsi.html

find . -name "*.log" -type f
来源：http://hz.yj202588.top/gtweztziaq.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtpovueiav.html

find . -mtime -7 -type f
来源：http://hz.zhaomingkeji.xyz/gtfauysvka.html

[R45] 批量删除
来源：http://hz.bjfxy.top/gtazijttjd.html

find . -name "*.tmp" -delete
来源：http://hz.dianchejie.cn/gttoeyycmc.html

[R46] 递归替换文件内容
来源：http://hz.xingfuxueyuan.xyz/gthdpnshtp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenjidiqi.icu/gtbgqtgpyt.html

[R47] sed 单行替换
来源：http://hz.yueranfly.top/gtxovmjmvk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dianchejie.cn/gttkiwpwdm.html

[R48] awk 取指定列
来源：http://hz.meibo888.top/gtkkhrudra.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxuanxn.top/gtyubifmfa.html

[R49] awk 带条件
来源：http://hz.ppjwa.cn/gtzlxozcno.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gtqgbmbfvh.html

[R50] awk 求和
来源：http://hz.hfpthk.cn/gtfnfzaxyl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sweek.top/gthmaxpigg.html

[R51] 排序去重取前几
来源：http://hz.52xcode.cn/gtmdlznqzl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtnrczmnkd.html

[R52] 统计行数
来源：http://hz.chenlongwang.top/gtvlhxapdc.html

wc -l a.txt
来源：http://hz.shanyushiyangkeji.top/gtprkagopq.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtvnpoliqy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtmzkibmwo.html

[R54] 比较两个文件
来源：http://hz.zdqjudy.top/gtthlhdrks.html

diff a.txt b.txt
来源：http://hz.jinyuanbaomall.cn/gteyqwvwgn.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gteocihpvw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tianlin.xyz/gttwriojwm.html

[R56] 远程拷贝
来源：http://hz.ydjk.org.cn/gtbljnrfwn.html

scp file user@host:/path/
来源：http://hz.c1oappe.top/gtetnfeegk.html

[R57] 远程执行命令
来源：http://hz.yj20258888.top/gtdkcxfhnr.html

ssh user@host 'uptime'
来源：http://hz.jinyuanbaomall.cn/gtrwaolvsa.html

[R58] 下载文件
来源：http://hz.pengpengdd.cyou/gtnkhxnvzf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tanke756.top/gtkqmjhebj.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtqeacbufl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtlkyzgvah.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtndbaougr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinghuilouyu.cn/gtogtxbcnc.html

[R61] 磁盘占用
来源：http://hz.sweek.top/gtafchtsnh.html

df -h;  du -sh *
来源：http://hz.smart0.xyz/gtgbpzhgaq.html

[R62] 找最占空间的文件
来源：http://hz.cucudq.cn/gtfnwzjhyf.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtycsjxeiv.html

[R63] 内存与进程
来源：http://hz.xylfe.cn/gtthjwcqji.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtjigxqcqv.html

[R64] 结束进程
来源：http://hz.52xcode.cn/gtsnwlghob.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jianghu66.top/gtuimmceyn.html

[R65] 查看端口占用
来源：http://hz.zhixingplan.top/gttzxfgifp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangtech.top/gtzmycvpsd.html

[R66] 定时任务
来源：http://hz.birdmap.top/gtouymbulb.html

crontab -e;  crontab -l
来源：http://hz.bjfxy.top/gtvgjvufne.html

[R67] 生成随机十六进制串
来源：http://hz.kuanghao11.cn/gtbyvicopo.html

openssl rand -hex 16
来源：http://hz.yvedp.cn/gtcdnwlqxr.html

[R68] 计算文件校验值
来源：http://hz.sufxvd.cn/gtthrgslmj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhongyouzk.top/gtsaaxhpgw.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtwfvenmaf.html

head -c 16 /dev/urandom | base64
来源：http://hz.birdmap.top/gtzmxxrcyb.html

[R70] 时间戳与互转
来源：http://hz.zhijiandao.cn/gtdzszoexi.html

date +%s;  date -d @1700000000
来源：http://hz.nanxinkj.top/gtljzwqaud.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtnlvpeemi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sweek.top/gtmjkbbijm.html

[R72] 等待端口就绪
来源：http://hz.hnqzz.top/gtjettqkhy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.haohaochexian.top/gtplquoghi.html

[R73] 分割大日志
来源：http://hz.shanyushiyangkeji.top/gtowafttli.html

split -l 1000 big.log part_
来源：http://hz.cucudq.cn/gtmrrjujwl.html

[R74] 批量重命名
来源：http://hz.hnxiangtu.top/gtanbplbmx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtdhbdtpnr.html

[R75] 导出环境变量
来源：http://hz.gogol.net.cn/gtzpweedvn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtvggtnnzi.html

[R76] 使用临时文件
来源：http://hz.ehwqpu.com/gtvwnnhtct.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuanzhike.top/gtodjvjoeo.html

[R77] 读取用户输入
来源：http://hz.wangshuangyany.cn/gtcgenxtza.html

read -rp "请输入: " ans
来源：http://hz.smart0.xyz/gtxggsspmx.html

[R78] 交互式菜单
来源：http://hz.daxiang520.top/gtkqgtnsbx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.316326.xyz/gtbdxclhtw.html

[R79] 解析命令行选项
来源：http://hz.nanxinkj.top/gtyyqaacyq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenlongwang.top/gtzjsdaees.html

[R80] 查看脚本执行耗时
来源：http://hz.shuidangran.top/gtuqncitwo.html

time ./run.sh
来源：http://hz.tian-w.cn/gtlcagxcta.html

================================================================================
来源：http://hz.hywenlv.cn/gtsnpuswyt.html

S. C / C++ 专题
来源：http://hz.guannengcc.top/gtripsbyyf.html

================================================================================
来源：http://hz.xylfe.cn/gtjefybotf.html

[S01] C：Hello World
来源：http://hz.nwbrower.top/gttsmugypx.html

#include <stdio.h>
来源：http://hz.svipenyu.cn/gtkitmlvoc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.iojbl.cn/gtlovckdeu.html

[S02] C：变量与格式化输出
来源：http://hz.kuanghao11.cn/gtvdglicls.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtqiafygrv.html

[S03] C：读入整数
来源：http://hz.cashguo.top/gtoqyslbbs.html

int x; scanf("%d", &x);
来源：http://hz.nanxinkj.top/gtmzmokhlw.html

[S04] C：字符串复制
来源：http://hz.yj20258.top/gtwpgajqlz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtiwyxkjdd.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtruqczoty.html

strlen(s)
来源：http://hz.dianchejie.cn/gtwhoxfhxu.html

[S06] C：字符串比较
来源：http://hz.jinghuilouyu.cn/gtthnmdpzx.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gtjbswlcvs.html

[S07] C：数组遍历求和
来源：http://hz.gaohongyu789.top/gtqqlsipeh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtiiibpwcg.html

[S08] C：动态内存分配与释放
来源：http://hz.yvedp.cn/gtkquodzbt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.redwolf501.top/gtatbmdtjm.html

[S09] C：结构体定义与初始化
来源：http://hz.ehwqpu.com/gttlwbnhxi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtkirbderq.html

[S10] C：指针与解引用
来源：http://hz.0kj1m.cn/gtymoyhvrt.html

int *p = &a;  *p = 5;
来源：http://hz.xylfe.cn/gtkrfaplpc.html

[S11] C：逐行读文件
来源：http://hz.hnxiangtu.top/gtyqlwhktu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fzhhl.top/gteohtutlt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gzhubu.top/gtiwcyvtsd.html

fclose(f);
来源：http://hz.zycfv.cn/gtzixoldba.html

[S12] C：写文件
来源：http://hz.hysaishi.cn/gtyzkkxzgo.html


<!-- 参考信息 -->