代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.sxryk.cn/gtxigdwtbx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daxiang520.top/gtatiwczku.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sweek.top/gtdpuxflam.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gtxvwwaoww.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zycfv.cn/gtfvhiuvbj.html

[Q50] 批量更新
来源：http://hz.zhongyouzk.top/gtkwwvlgst.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hysaishi.cn/gtmeyyfekv.html

[Q51] 用子查询更新
来源：http://hz.ydjk.org.cn/gtjtwgkkxi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hfpthk.cn/gtcqmztvau.html

[Q52] 删除指定行
来源：http://hz.jianghu66.top/gtwnpcpysl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aibaodan.cn/gtdzuiysfb.html

[Q53] 按条件删除
来源：http://hz.fzhhl.top/gtctvdjtor.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hysaishi.cn/gtlhegllrj.html

[Q54] 清空表
来源：http://hz.sweek.top/gtqrhocaco.html

TRUNCATE TABLE logs;
来源：http://hz.yueranfly.top/gtgzrwvzrn.html

[Q55] 排名（并列占位）
来源：http://hz.jinghuilouyu.cn/gtddditeet.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jyoumei.cn/gtssvwpbqa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cqqwz.cn/gtbtcoqulf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenjidiqi.icu/gthatlsxtb.html

[Q57] 行号
来源：http://hz.cheryme.top/gtlyygkwmu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.mhx1999.top/gtpzxqvpsw.html

[Q58] 累计求和
来源：http://hz.smart0.xyz/gtuorrxjww.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnqzz.top/gtycrokkla.html

[Q59] 分组内累计
来源：http://hz.c1oappe.top/gtrmdiikih.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ehwqpu.com/gtxpojhvac.html

[Q60] 取上一行 / 下一行
来源：http://hz.shangyingyoupin.top/gtiruuaegu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangkeji.top/gthqmlkudq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuanzx.com/gtvkhjlycl.html

[Q61] 移动平均
来源：http://hz.jinqigufen.top/gtmvpjuerp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cheryme.top/gtlmqjcgjz.html

[Q62] 分组占比
来源：http://hz.xinyue.icu/gtqummixbn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtajubuxtq.html

[Q63] 开启事务
来源：http://hz.yongpay.top/gtwpentaqp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinyuanbaomall.cn/gtqobcqysn.html

[Q64] 提交事务
来源：http://hz.pengpengdd.cyou/gtofawzrnp.html

COMMIT;
来源：http://hz.sxryk.cn/gttkttavvu.html

[Q65] 回滚事务
来源：http://hz.sufxvd.cn/gtwiitoqfu.html

ROLLBACK;
来源：http://hz.jinghuilouyu.cn/gtjsjnlvba.html

[Q66] 行锁查询
来源：http://hz.zhongyouzk.top/gttciryrlr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cashguo.top/gtnghzpjkz.html

[Q67] 设置隔离级别
来源：http://hz.zdqjudy.top/gtzsymoyzg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jlsjyb.cn/gtomaeuptt.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtldwalcdl.html

SAVEPOINT sp1;
来源：http://hz.yj20258888.top/gtyxlrnikk.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtnmsyzjzu.html

[Q69] 查看执行计划
来源：http://hz.hysaishi.cn/gtmbijyxlz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhongyouzk.top/gtracofhdp.html

[Q70] 更新统计信息
来源：http://hz.quarkkingdee.top/gtbfjgxtwj.html

ANALYZE TABLE users;
来源：http://hz.iojbl.cn/gtrzfshwaw.html

[Q71] 查看建表语句
来源：http://hz.zhengqikj.top/gtdunrfwnk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258888.top/gtoukjnnpr.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gtkazoogto.html

SHOW INDEX FROM users;
来源：http://hz.zhoulong.xyz/gtgihymyfe.html

[Q73] 查看表状态
来源：http://hz.cqqwz.cn/gtevxwrheo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tianlin.xyz/gtlmqrdbyc.html

[Q74] 强制使用索引
来源：http://hz.ivvv.top/gtuasmvhss.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhixingplan.top/gtprejjqqa.html

[Q75] 日期格式化
来源：http://hz.xuetiantiany.cn/gtelzlapsd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dianchejie.cn/gtxcdfhpze.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinyuanbaomall.cn/gtaxyhvbjb.html

[Q76] 按天统计
来源：http://hz.hammf.cn/gtsrtsyorc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guannengcc.top/gtfdvtufke.html

[Q77] 时间加减
来源：http://hz.xuetiantiany.cn/gtbfuhlxdo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.316326.xyz/gtmumifutn.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gtdprwmvnv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.quarkkingdee.top/gtqkqjuxxo.html

[Q79] 字符串拼接
来源：http://hz.daria6918.cn/gtwhgnvydv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.andypj.xyz/gtiaxneomn.html

[Q80] 字符串截取
来源：http://hz.birdmap.top/gthwnkouws.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xinyue.icu/gtjghkssbu.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtexmfhplb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aizwys.cn/gtpfewworr.html

[Q82] 字符长度与字节长度
来源：http://hz.pycfn.com/gttuejzrfe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xinyue.icu/gtgxeqgrdz.html

[Q83] 大小写转换
来源：http://hz.birdmap.top/gtgfigkxfg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jianghu66.top/gtkmioxcgy.html

[Q84] 去除首尾空格
来源：http://hz.shzxlz.cn/gtqnnwsqtu.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtnmjeeouk.html

[Q85] 数值取整
来源：http://hz.jiagoushi.top/gtidfrtwuu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.c1oappe.top/gtfisokonf.html

[Q86] 读取 JSON 字段
来源：http://hz.xziqi.cn/gtoukbnune.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhaomingkeji.xyz/gtfihmvpmy.html

[Q87] JSON 字段做条件
来源：http://hz.quarkkingdee.top/gtqongkpke.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhaomingkeji.xyz/gtruzfqekp.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenlongwang.top/gtjscnojei.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cashguo.top/gtsdkhmjrs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gtohrbnoig.html

[Q89] 判断表是否存在
来源：http://hz.cashguo.top/gtfnsfghrp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gtycbujyie.html

[Q90] 生成序号列
来源：http://hz.tian-w.cn/gtrhwihdmj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yonumen.top/gtciqrwhxi.html

================================================================================
来源：http://hz.jinqigufen.top/gtcjpscmux.html

R. Bash 专题
来源：http://hz.zhaomingkeji.xyz/gtisbaheym.html

================================================================================
来源：http://hz.hnxiangtu.top/gtxsxffkig.html

[R01] shebang 与严格模式
来源：http://hz.pengpengdd.cyou/gtdoxtnyip.html

#!/usr/bin/env bash
来源：http://hz.yueranfly.top/gtslfasllt.html

set -euo pipefail
来源：http://hz.jinghuilouyu.cn/gtnnlgarer.html

[R02] 变量赋值与使用
来源：http://hz.jinghuilouyu.cn/gtzgvppbfh.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gtfuqptgus.html

[R03] 只读变量
来源：http://hz.shanyushiyangkeji.top/gtwfwfvvjp.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtzgivsfnp.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gtgywsyinz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenzaomai.com/gthifrmjmv.html

[R05] 参数默认值
来源：http://hz.ehwqpu.com/gtatexejcf.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtjawrvija.html

[R06] 判断命令是否存在
来源：http://hz.xziqi.cn/gthaakixjj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258.top/gtjqirvegl.html

[R07] if 判断文件
来源：http://hz.redwolf501.top/gtdnxgidqd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sufxvd.cn/gtloxrmxze.html

[R08] 数值比较
来源：http://hz.cucudq.cn/gtypalssaz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daxiang520.top/gtwviuvpav.html

[R09] 字符串比较
来源：http://hz.xziqi.cn/gtepquwbmc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shzxlz.cn/gtjvihqssr.html

[R10] 正则匹配
来源：http://hz.zhongyouzk.top/gtplhsawgp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangtech.top/gtxndytqrj.html

[R11] case 多分支
来源：http://hz.bjfxy.top/gtnfawodex.html

case "$1" in
来源：http://hz.shzxlz.cn/gtydyaxajy.html

start) echo "启动" ;;
来源：http://hz.yvedp.cn/gtznfbrjyb.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gtpmuicapu.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gthbtzartu.html

esac
来源：http://hz.xylfe.cn/gtyfislgaa.html

[R12] for 遍历文件
来源：http://hz.ehwqpu.com/gtnoyruxgi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.quarkkingdee.top/gtacogkfuf.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gtienrrpbh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ywan-chungtsiang.top/gtybpwxyzh.html

[R14] C 风格 for
来源：http://hz.fzhhl.top/gtglrxxlxu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dashuyun.cn/gtflpfpojr.html

[R15] while 逐行读文件
来源：http://hz.nanxinkj.top/gtmakhcrxg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtikgslpuh.html

[R16] until 等待条件
来源：http://hz.pycfn.com/gtiukyikte.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tian-w.cn/gtcocoaurl.html

[R17] 数组定义与取值
来源：http://hz.yangfankeji.com/gtahmioqne.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nwbrower.top/gtyyqiclnw.html

[R18] 遍历数组
来源：http://hz.havefunace.top/gtnwyxlkhd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.andypj.xyz/gtfxmzjlrd.html

[R19] 数组长度
来源：http://hz.andypj.xyz/gtrbjzzvkz.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtbvppvmaz.html

[R20] 关联数组（字典）
来源：http://hz.shangyingyoupin.top/gtkdbezvwv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tian-w.cn/gtuvssutqw.html

[R21] 字符串长度
来源：http://hz.yj20258888.top/gtwmdzsmor.html

echo "${#s}"
来源：http://hz.fzhhl.top/gtawosdylk.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtbaotkngw.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gtiqsgdcdu.html

[R23] 字符串替换
来源：http://hz.chenlongwang.top/gtabtpmish.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.kuanghao11.cn/gtcpalztqh.html

[R24] 大小写转换
来源：http://hz.tian-w.cn/gtdenonwrv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jiagoushi.top/gtaobphidm.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgufenzy.top/gtjnjtiocw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aibaodan.cn/gtkhwahape.html

[R26] 命令替换
来源：http://hz.jinghuilouyu.cn/gtnlnapbok.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtpirbmbol.html

[R27] 算术展开
来源：http://hz.yanxiufei.cn/gtlhezotkx.html

echo $((1 + 2 * 3))
来源：http://hz.feifeiyinyue.top/gtyqhzcavp.html

[R28] 浮点运算
来源：http://hz.hammf.cn/gtjxkaapwu.html

echo "scale=2; 10/3" | bc
来源：http://hz.dianchejie.cn/gtyeygijgb.html

[R29] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtfitzhxze.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtluyjwduo.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gtjpjforve.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cashguo.top/gtbydwysbm.html

[R31] 局部变量
来源：http://hz.xingfuxueyuan.xyz/gtpeiuyhwz.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangtech.top/gtahdjokhe.html

[R32] 参数个数校验
来源：http://hz.9152youxi.cn/gtbywuqtft.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cashguo.top/gtqrggsfwe.html

[R33] 捕获错误并提示行号
来源：http://hz.dianchejie.cn/gtrsimcvgj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgufenzy.top/gtyyhhcimx.html

[R34] 退出时清理
来源：http://hz.redwolf501.top/gtwkqjyknv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtaaqmztix.html

[R35] 后台执行并等待
来源：http://hz.xingfuxueyuan.xyz/gtlehedkjc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yongpay.top/gtsmwwivoa.html

[R36] 并发执行多个任务
来源：http://hz.zycfv.cn/gtlxyhukcq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.meibo888.top/gtswrtqvks.html

[R37] 把输出赋给变量
来源：http://hz.vqdsnc.cn/gtiwjznyrp.html

files=$(ls -1)
来源：http://hz.yj20258888.top/gtcczinymu.html

[R38] 管道串联
来源：http://hz.birdmap.top/gttekpkduw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.0kj1m.cn/gtjlsujize.html

[R39] 重定向标准输出与错误
来源：http://hz.52xcode.cn/gtnuudrnam.html

cmd > out.log 2>&1
来源：http://hz.ydzc1.top/gtlrfvacyg.html

[R40] 追加写日志
来源：http://hz.hongshengwenyu.top/gtxflamijx.html

echo "log" >> out.log
来源：http://hz.guowangkeji.top/gtvksrvmmo.html

[R41] 丢弃输出
来源：http://hz.ydjk.org.cn/gtzxowmtrt.html

cmd >/dev/null 2>&1
来源：http://hz.yvedp.cn/gtkkynunak.html

[R42] 输入重定向
来源：http://hz.ehwqpu.com/gtqsfupdal.html

wc -l < a.txt
来源：http://hz.ydzc1.top/gtpuxrbcqa.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gtvbbvsgsk.html

find . -name "*.log" -type f
来源：http://hz.havefunace.top/gtcihqxveo.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtihvszudx.html

find . -mtime -7 -type f
来源：http://hz.hfpthk.cn/gtkyeyjajr.html

[R45] 批量删除
来源：http://hz.shuidangran.top/gttjqgrmpm.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtcitmydgb.html

[R46] 递归替换文件内容
来源：http://hz.guowangkeji.top/gteahlftle.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guannengcc.top/gtloyirlmv.html

[R47] sed 单行替换
来源：http://hz.zycfv.cn/gtcymbglsg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ppjwa.cn/gtccvbmmyi.html

[R48] awk 取指定列
来源：http://hz.yuanzhike.top/gtsmxplszl.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnxiangtu.top/gtoscddzam.html

[R49] awk 带条件
来源：http://hz.birdmap.top/gthvptwijn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fzhhl.top/gtdmpgneku.html

[R50] awk 求和
来源：http://hz.zdqjudy.top/gtytqbhofl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jiagoushi.top/gtvwulgjia.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gtdznvbxlp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ywan-chungtsiang.top/gtnheypllx.html

[R52] 统计行数
来源：http://hz.hywenlv.cn/gtphdhtpjv.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtvewpjoeb.html

[R53] 查看文件头与实时尾
来源：http://hz.yanxiufei.cn/gtdllktzkr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hywenlv.cn/gtimdclnqb.html

[R54] 比较两个文件
来源：http://hz.c1oappe.top/gtvxfngise.html

diff a.txt b.txt
来源：http://hz.aibaodan.cn/gtltilcvdz.html

[R55] 压缩与解压
来源：http://hz.52xcode.cn/gtdzpnyrtc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.feifeiyinyue.top/gtkfaelxul.html

[R56] 远程拷贝
来源：http://hz.tanke756.top/gtiglvlvbi.html

scp file user@host:/path/
来源：http://hz.hammf.cn/gtijzuizlp.html

[R57] 远程执行命令
来源：http://hz.mhx1999.top/gteelmoyek.html

ssh user@host 'uptime'
来源：http://hz.ivvv.top/gtsnktpumo.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtyrvyvnub.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ppjwa.cn/gttiuprgff.html

[R59] 发 POST JSON
来源：http://hz.yj20258888.top/gtnjbwzxwc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xingfuxueyuan.xyz/gtncyrplgx.html

[R60] 只看 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtazjjrual.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cucudq.cn/gtincnwjsc.html

[R61] 磁盘占用
来源：http://hz.zhoulong.xyz/gtqnvwpsxe.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtwfntswez.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gtegonrqds.html

du -ah . | sort -rh | head -10
来源：http://hz.zhengqikj.top/gtgpjgswkj.html

[R63] 内存与进程
来源：http://hz.cdnleiting.top/gtyrojabck.html

free -h;  ps aux | grep nginx
来源：http://hz.haohaochexian.top/gtlfjyhzzo.html

[R64] 结束进程
来源：http://hz.shanyushiyangtech.top/gtaanqufeu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenjidiqi.icu/gtgwyqhglo.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gtibqihpma.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gttatmdlyg.html

[R66] 定时任务
来源：http://hz.hnqzz.top/gthyuqvjem.html

crontab -e;  crontab -l
来源：http://hz.shzxlz.cn/gtwyqwzqnx.html

[R67] 生成随机十六进制串
来源：http://hz.xylfe.cn/gtfrgchwue.html

openssl rand -hex 16
来源：http://hz.ybcxt.top/gtthexwsze.html

[R68] 计算文件校验值
来源：http://hz.snrcjt.cn/gtrtrojqpt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cheryme.top/gtxxfpedrt.html

[R69] 生成随机密码
来源：http://hz.bjfxy.top/gttzxagklr.html

head -c 16 /dev/urandom | base64
来源：http://hz.cheryme.top/gtsheytucy.html

[R70] 时间戳与互转
来源：http://hz.zhengqikj.top/gtlrckmvmh.html

date +%s;  date -d @1700000000
来源：http://hz.quarkkingdee.top/gtpbbzmqse.html

[R71] 日期格式化
来源：http://hz.zdqjudy.top/gteomjtnxc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.0kj1m.cn/gtjouipfno.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtkmkvdyvl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ivvv.top/gthidqqzzd.html

[R73] 分割大日志
来源：http://hz.zhengqikj.top/gtovyscwze.html

split -l 1000 big.log part_
来源：http://hz.ydjk.org.cn/gtboknomqy.html

[R74] 批量重命名
来源：http://hz.yanxiufei.cn/gtecjfxxie.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gtqxwsjjgm.html

[R75] 导出环境变量
来源：http://hz.smart0.xyz/gtskpzunpf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guowangkeji.top/gttvvtrusn.html

[R76] 使用临时文件
来源：http://hz.redwolf501.top/gtivdpwsui.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtguoublqc.html

[R77] 读取用户输入
来源：http://hz.yuanzhike.top/gtsgugozfs.html

read -rp "请输入: " ans
来源：http://hz.xuanzx.com/gtujzghowh.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtfpusargo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinyuanbaomall.cn/gtyizcsjgu.html

[R79] 解析命令行选项
来源：http://hz.chenlongwang.top/gtljmdhqyd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yueranfly.top/gtwuqrnytz.html

[R80] 查看脚本执行耗时
来源：http://hz.fengsongda.top/gtksqyfkcm.html

time ./run.sh
来源：http://hz.yueranfly.top/gtpvxrsqsp.html

================================================================================
来源：http://hz.snrcjt.cn/gtliukqmsl.html

S. C / C++ 专题
来源：http://hz.sweek.top/gtfriwyhrs.html

================================================================================
来源：http://hz.jinqigfzy.top/gtihgzrjur.html

[S01] C：Hello World
来源：http://hz.yuanzhike.top/gtxvnbrebs.html

#include <stdio.h>
来源：http://hz.yuanzhike.top/gtniaeesgc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pycfn.com/gtybccwflm.html

[S02] C：变量与格式化输出
来源：http://hz.jlsjyb.cn/gtopgiussx.html

int a = 10; printf("%d\n", a);
来源：http://hz.yueranfly.top/gtpquzsikb.html

[S03] C：读入整数
来源：http://hz.ppjwa.cn/gtggafmrrc.html

int x; scanf("%d", &x);
来源：http://hz.cheryme.top/gtbiqogyou.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtaypqskyn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenlongwang.top/gtwqlkgaud.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtdaslnnzr.html

strlen(s)
来源：http://hz.guannengcc.top/gtuvuidoqm.html

[S06] C：字符串比较
来源：http://hz.shangyingyoupin.top/gtqzcdgukb.html

strcmp(a, b) == 0
来源：http://hz.jqgfzy.top/gtcyeqadmy.html

[S07] C：数组遍历求和
来源：http://hz.xziqi.cn/gtmpgxikph.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jlsjyb.cn/gtiythadud.html

[S08] C：动态内存分配与释放
来源：http://hz.fzhhl.top/gtxprbpkod.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangtech.top/gtfhzfcvsp.html

[S09] C：结构体定义与初始化
来源：http://hz.yvedp.cn/gtwickgyhk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258.top/gteznwzmlk.html

[S10] C：指针与解引用
来源：http://hz.xziqi.cn/gtfgoekafo.html

int *p = &a;  *p = 5;
来源：http://hz.hywenlv.cn/gtflyiutsa.html

[S11] C：逐行读文件
来源：http://hz.gotoacloud.top/gtmrmhmfzq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhongyouzk.top/gtezmlptiy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtsgnpvohg.html

fclose(f);
来源：http://hz.hfpthk.cn/gtvsydzaqp.html

[S12] C：写文件
来源：http://hz.zhaomingkeji.xyz/gtzvwsausr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gtawjjlgnb.html

[S13] C：宏定义
来源：http://hz.hnxiangtu.top/gtvblbggjx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yangfankeji.com/gtleudepxn.html

[S14] C：枚举
来源：http://hz.hnqzz.top/gtwrunqunk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gzhubu.top/gtdkxtqjlg.html

[S15] C：类型转换
来源：http://hz.fzhhl.top/gtkvzxagoh.html

(double) a / b
来源：http://hz.andypj.xyz/gtziekcfxm.html

[S16] C：位操作置位
来源：http://hz.yonumen.top/gtvvheayla.html

x |= (1 << 3);
来源：http://hz.guannengcc.top/gtycqzkmkw.html

[S17] C：安全拼接字符串
来源：http://hz.c1oappe.top/gtfgqpgazp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fengsongda.top/gtzobaxnso.html

[S18] C：命令行参数
来源：http://hz.sweek.top/gtvkhdafpq.html


<!-- 参考信息 -->