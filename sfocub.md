代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.haohaochexian.top/gtpndykquo.html

[Q60] 取上一行 / 下一行
来源：http://hz.shuidangran.top/gtkuqdkitz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jlsjyb.cn/gtwdpsiskr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fzhhl.top/gtcskcsude.html

[Q61] 移动平均
来源：http://hz.jlsjyb.cn/gtwchsllso.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.mhx1999.top/gtzpvqjioe.html

[Q62] 分组占比
来源：http://hz.havefunace.top/gtopmeadxz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtvtcqdvlr.html

[Q63] 开启事务
来源：http://hz.hnxiangtu.top/gtmxuhktog.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtdhoyholm.html

[Q64] 提交事务
来源：http://hz.zhongyouzk.top/gtmselocfj.html

COMMIT;
来源：http://hz.jqgufenzy.top/gtfkjenqij.html

[Q65] 回滚事务
来源：http://hz.xziqi.cn/gthluswezo.html

ROLLBACK;
来源：http://hz.yj20258888.top/gtghqylsyw.html

[Q66] 行锁查询
来源：http://hz.gogol.net.cn/gtnokwmptw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ppjwa.cn/gttwocndgs.html

[Q67] 设置隔离级别
来源：http://hz.vqdsnc.cn/gtnwmebceg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.fengsongda.top/gtxxizjzrs.html

[Q68] 保存点
来源：http://hz.hongshengwenyu.top/gtzqfvvccm.html

SAVEPOINT sp1;
来源：http://hz.xinyue.icu/gtqpshfwqy.html

ROLLBACK TO sp1;
来源：http://hz.cashguo.top/gthdfofpgk.html

[Q69] 查看执行计划
来源：http://hz.tian-w.cn/gtmnvhwqgg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pengpengdd.cyou/gtgbmkgycf.html

[Q70] 更新统计信息
来源：http://hz.52xcode.cn/gtzfbcgpvr.html

ANALYZE TABLE users;
来源：http://hz.zhengqikj.top/gtdyiymwmp.html

[Q71] 查看建表语句
来源：http://hz.gaohongyu789.top/gtekpghlqj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yonumen.top/gtkesrkuxl.html

[Q72] 查看索引
来源：http://hz.haohaochexian.top/gtqcbsrptp.html

SHOW INDEX FROM users;
来源：http://hz.aizwys.cn/gtcqhskykr.html

[Q73] 查看表状态
来源：http://hz.hysaishi.cn/gtbbrsqoex.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.9152youxi.cn/gtaqgdcqls.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtzkmgxrqh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hammf.cn/gtcbjfdmst.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gtkwkygbbt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinqigfzy.top/gtcloyczqg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gtgechjypb.html

[Q76] 按天统计
来源：http://hz.chenzaomai.com/gticeokjhp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuetiantiany.cn/gtwgwytrmb.html

[Q77] 时间加减
来源：http://hz.tianlin.xyz/gtubdfblyl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.c1oappe.top/gtzstuxaxq.html

[Q78] 当前时间
来源：http://hz.pengpengdd.cyou/gtwzgdkaas.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.vqdsnc.cn/gtklwibzpp.html

[Q79] 字符串拼接
来源：http://hz.hnxiangtu.top/gtizwpyvbo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daxiang520.top/gtxnstfqdj.html

[Q80] 字符串截取
来源：http://hz.cdnleiting.top/gtrhrmpjxw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cucudq.cn/gtigjjcsuz.html

[Q81] 字符串替换
来源：http://hz.iojbl.cn/gtwanjuaiy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cucudq.cn/gtwzlgycux.html

[Q82] 字符长度与字节长度
来源：http://hz.zhiwuduotai.top/gtftijzaqg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shuidangran.top/gtuheetlwm.html

[Q83] 大小写转换
来源：http://hz.yvedp.cn/gtdffxunkf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ppjwa.cn/gtwhuphguv.html

[Q84] 去除首尾空格
来源：http://hz.52xcode.cn/gtemorrzsn.html

SELECT TRIM(name) FROM users;
来源：http://hz.iojbl.cn/gtkkdfiupa.html

[Q85] 数值取整
来源：http://hz.shzxlz.cn/gtmysymmlq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtpgbojeom.html

[Q86] 读取 JSON 字段
来源：http://hz.guannengcc.top/gtkgonrepx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ydzc1.top/gtbtrstwll.html

[Q87] JSON 字段做条件
来源：http://hz.ehwqpu.com/gtdqmxsudc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sxryk.cn/gtebjgzjol.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangdashe.top/gthcgrlnrl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtaadtmfra.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gtrjwwfsia.html

[Q89] 判断表是否存在
来源：http://hz.quarkkingdee.top/gtadqgspqa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daxiang520.top/gtyramiyzy.html

[Q90] 生成序号列
来源：http://hz.shangyingyoupin.top/gtcuazeseb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtusjeuonj.html

================================================================================
来源：http://hz.c1oappe.top/gtfmlqxsda.html

R. Bash 专题
来源：http://hz.ybcxt.top/gtnsqhmzeh.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtpcneymgm.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gtszyaytlm.html

#!/usr/bin/env bash
来源：http://hz.ydzc1.top/gtwxbkuikc.html

set -euo pipefail
来源：http://hz.xziqi.cn/gtynramjbt.html

[R02] 变量赋值与使用
来源：http://hz.cheryme.top/gtqtkwosfa.html

name="Tom"; echo "$name"
来源：http://hz.9152youxi.cn/gtlhpqqdpw.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtlpunrkqi.html

readonly PI=3.14
来源：http://hz.dianchejie.cn/gtaznlgioc.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtcnmtzomr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtemhixjrj.html

[R05] 参数默认值
来源：http://hz.feifeiyinyue.top/gtexkihgkz.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtnuamkfah.html

[R06] 判断命令是否存在
来源：http://hz.c1oappe.top/gtymyfpyoo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ehwqpu.com/gtadfbvhme.html

[R07] if 判断文件
来源：http://hz.9152youxi.cn/gtofwqmydy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinghuilouyu.cn/gtmseyyjvg.html

[R08] 数值比较
来源：http://hz.0kj1m.cn/gtjiuubzvg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gogol.net.cn/gtcinikqff.html

[R09] 字符串比较
来源：http://hz.pengpengdd.cyou/gtmqaxqtyt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gtxpvkayuz.html

[R10] 正则匹配
来源：http://hz.nwbrower.top/gtdqdtcvwq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtuhtryxot.html

[R11] case 多分支
来源：http://hz.jlsjyb.cn/gtcivyiqig.html

case "$1" in
来源：http://hz.yangfankeji.com/gtmmkimdrc.html

start) echo "启动" ;;
来源：http://hz.shangyingyoupin.top/gtuefacjhp.html

stop)  echo "停止" ;;
来源：http://hz.xuetiantiany.cn/gtidbbkuhp.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtilwmqzhu.html

esac
来源：http://hz.jinyuanbaomall.cn/gtrlnpbnpj.html

[R12] for 遍历文件
来源：http://hz.aizwys.cn/gttigjajaw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cqqwz.cn/gtwhcvxxgr.html

[R13] for 计数循环
来源：http://hz.hammf.cn/gtznnymzgc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.316326.xyz/gtcthzjzwt.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gtjljsmpsi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.havefunace.top/gtgbskhulu.html

[R15] while 逐行读文件
来源：http://hz.yuanzhike.top/gtdoeygdou.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nwbrower.top/gtpqhemzva.html

[R16] until 等待条件
来源：http://hz.zhengqikj.top/gtnlwahnqw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxuanxn.top/gtaoozmgtz.html

[R17] 数组定义与取值
来源：http://hz.0kj1m.cn/gtjkkqydxd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydzc1.top/gtgicarozg.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtokbqtjgn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtyzdwzvxl.html

[R19] 数组长度
来源：http://hz.tian-w.cn/gtsfibramx.html

echo "${#arr[@]}"
来源：http://hz.tanke756.top/gtrpysjczf.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtujbacbiw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.bjfxy.top/gtgwqeubys.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtwhqmumja.html

echo "${#s}"
来源：http://hz.svipenyu.cn/gtqwnhcwca.html

[R22] 截取子串
来源：http://hz.jiagoushi.top/gtiapjvzhl.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gttsxlqgal.html

[R23] 字符串替换
来源：http://hz.yueranfly.top/gtfwduvdhc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhaomingkeji.xyz/gtsgcpfsui.html

[R24] 大小写转换
来源：http://hz.fengsongda.top/gtfsjdxdjn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aibaodan.cn/gtuncxeffo.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenjidiqi.icu/gtjllqghib.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtihjpzjew.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gtqnilkwcl.html

now=$(date +%F); echo "$now"
来源：http://hz.quarkkingdee.top/gtqmubdfar.html

[R27] 算术展开
来源：http://hz.jinqigufen.top/gtxeigypmi.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtkvfcpvmg.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtabamgpwd.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinyuanbaomall.cn/gtpoxruhwk.html

[R29] 定义函数
来源：http://hz.jianghu66.top/gtsnzhzett.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.316326.xyz/gtnzdumluw.html

[R30] 函数返回状态码
来源：http://hz.xylfe.cn/gtbpoitmzo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hongshengwenyu.top/gtzkrnsjpr.html

[R31] 局部变量
来源：http://hz.jinqigfzy.top/gtwkkptqsu.html

f() { local x=1; echo "$x"; }
来源：http://hz.bjfxy.top/gtdsmttpvi.html

[R32] 参数个数校验
来源：http://hz.tanke756.top/gtiuxocfui.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sufxvd.cn/gtlczqiiyi.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gtocampzcj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hfpthk.cn/gtuhdxoren.html

[R34] 退出时清理
来源：http://hz.zdqjudy.top/gtdeotbmeb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gttzcebckp.html

[R35] 后台执行并等待
来源：http://hz.ybcxt.top/gtkfuibgfb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yangfankeji.com/gtqgzyhudk.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtdearmgqw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xinyue.icu/gtgvksstnh.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtmkewjmdf.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtypshqxle.html

[R38] 管道串联
来源：http://hz.quarkkingdee.top/gtsnjzlpku.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hysaishi.cn/gtirnyzicq.html

[R39] 重定向标准输出与错误
来源：http://hz.chenjidiqi.icu/gtpurihbvq.html

cmd > out.log 2>&1
来源：http://hz.xinyue.icu/gtjghnenwb.html

[R40] 追加写日志
来源：http://hz.hongshengwenyu.top/gtjqrmygrq.html

echo "log" >> out.log
来源：http://hz.hfpthk.cn/gtcvltscla.html

[R41] 丢弃输出
来源：http://hz.yvedp.cn/gtifdezats.html

cmd >/dev/null 2>&1
来源：http://hz.xziqi.cn/gtkzipthxb.html

[R42] 输入重定向
来源：http://hz.meibo888.top/gtinukilyy.html

wc -l < a.txt
来源：http://hz.hammf.cn/gtzpymkyue.html

[R43] 按名字查找文件
来源：http://hz.hnxiangtu.top/gtvnufeasg.html

find . -name "*.log" -type f
来源：http://hz.yonumen.top/gtujozpowr.html

[R44] 按修改时间查找
来源：http://hz.quarkkingdee.top/gtukoqplgk.html

find . -mtime -7 -type f
来源：http://hz.meibo888.top/gtjttbwbgx.html

[R45] 批量删除
来源：http://hz.sufxvd.cn/gtcliewuef.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtpqduvjpq.html

[R46] 递归替换文件内容
来源：http://hz.gotoacloud.top/gtvhipenyd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.haohaochexian.top/gtenbpbtaz.html

[R47] sed 单行替换
来源：http://hz.wangdashe.top/gtlczvuxcy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxuanxn.top/gtcrmvnuwj.html

[R48] awk 取指定列
来源：http://hz.chenjidiqi.icu/gtspchmakj.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgfzy.top/gtulioepga.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtxdqlygdg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtwjcqcrda.html

[R50] awk 求和
来源：http://hz.yangfankeji.com/gtznwwgxwb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangtech.top/gtnkjjaags.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gtpfgmudxc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xziqi.cn/gthjkmuihu.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtxoqegfqk.html

wc -l a.txt
来源：http://hz.cheryme.top/gtylbkvayg.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtfxmvvblz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuanzx.com/gtremxgmpc.html

[R54] 比较两个文件
来源：http://hz.zhijiandao.cn/gttmawrhau.html

diff a.txt b.txt
来源：http://hz.pycfn.com/gthlywnvht.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtxdxejpwt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sufxvd.cn/gtfgbczvlx.html

[R56] 远程拷贝
来源：http://hz.jinqigufen.top/gtwlkdooie.html

scp file user@host:/path/
来源：http://hz.redwolf501.top/gtjrdjdiyv.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtbklaeivq.html

ssh user@host 'uptime'
来源：http://hz.aibaodan.cn/gtevvnqqnb.html

[R58] 下载文件
来源：http://hz.cheryme.top/gtumldzdyp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuxming.cn/gtajfyavwz.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gtfgkcifgp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtxpemddpz.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtldccgigs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ppjwa.cn/gtasisqbrn.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gtgiuqbihx.html

df -h;  du -sh *
来源：http://hz.yangfankeji.com/gtecpfcgqo.html

[R62] 找最占空间的文件
来源：http://hz.hammf.cn/gtptyaswpx.html

du -ah . | sort -rh | head -10
来源：http://hz.jianghu66.top/gtxzyqczwy.html

[R63] 内存与进程
来源：http://hz.sweek.top/gtdgalroqv.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gtttxipnbw.html

[R64] 结束进程
来源：http://hz.iojbl.cn/gtkrgqnnvh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yanxiufei.cn/gtxzpkdwcr.html

[R65] 查看端口占用
来源：http://hz.xingfuxueyuan.xyz/gtagxdapho.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtadbwxznm.html

[R66] 定时任务
来源：http://hz.gaohongyu789.top/gtolapgupa.html

crontab -e;  crontab -l
来源：http://hz.xuetiantiany.cn/gtvacjcxqv.html

[R67] 生成随机十六进制串
来源：http://hz.hnxiangtu.top/gtqjyudlsr.html

openssl rand -hex 16
来源：http://hz.nanxinkj.top/gthsjtgmuv.html

[R68] 计算文件校验值
来源：http://hz.wangdashe.top/gtaavvvews.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yueranfly.top/gtsmpmevxo.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gtuzgcfdrd.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigfzy.top/gtdthuzetq.html

[R70] 时间戳与互转
来源：http://hz.jqgufenzy.top/gtkwlkltfd.html

date +%s;  date -d @1700000000
来源：http://hz.cucudq.cn/gturuwihvn.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtureabbyv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yongpay.top/gtiitoocqy.html

[R72] 等待端口就绪
来源：http://hz.jianghu66.top/gtnfdgxioj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nanxinkj.top/gtjqybxpbc.html

[R73] 分割大日志
来源：http://hz.ppjwa.cn/gthstzbyjg.html

split -l 1000 big.log part_
来源：http://hz.sysykeji.top/gtootkkrhc.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtoorefsjc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nwbrower.top/gthrvximtf.html

[R75] 导出环境变量
来源：http://hz.cheryme.top/gtzdboqccg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gtexjnpinf.html

[R76] 使用临时文件
来源：http://hz.xingfuxueyuan.xyz/gtqrixniet.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtoqusaqcg.html

[R77] 读取用户输入
来源：http://hz.chenlongwang.top/gtiobllxqp.html

read -rp "请输入: " ans
来源：http://hz.jinqigufen.top/gtagrwgxal.html

[R78] 交互式菜单
来源：http://hz.daria6918.cn/gtpoqbklfg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.andypj.xyz/gtoutjycrv.html

[R79] 解析命令行选项
来源：http://hz.hywenlv.cn/gtercclene.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nanxinkj.top/gtfkvskzoh.html

[R80] 查看脚本执行耗时
来源：http://hz.xuanzx.com/gtekrzdefn.html

time ./run.sh
来源：http://hz.hongshengwenyu.top/gtdndrxonu.html

================================================================================
来源：http://hz.cqqwz.cn/gtcfmstwbw.html

S. C / C++ 专题
来源：http://hz.yueranfly.top/gthndtaqkr.html

================================================================================
来源：http://hz.0kj1m.cn/gtafdspijr.html

[S01] C：Hello World
来源：http://hz.aizwys.cn/gtednauryh.html

#include <stdio.h>
来源：http://hz.hywenlv.cn/gtsgkytlmj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gotoacloud.top/gtdbkpyyhy.html

[S02] C：变量与格式化输出
来源：http://hz.redwolf501.top/gtppyhvgez.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtgczqovid.html

[S03] C：读入整数
来源：http://hz.dianchejie.cn/gtwsfxclpz.html

int x; scanf("%d", &x);
来源：http://hz.0kj1m.cn/gtfxknbovq.html

[S04] C：字符串复制
来源：http://hz.fzhhl.top/gtdlhhpmxq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ehwqpu.com/gthibzjxjk.html

[S05] C：字符串长度
来源：http://hz.fzhhl.top/gtyulizjxz.html

strlen(s)
来源：http://hz.zhijiandao.cn/gtuheqwtnw.html

[S06] C：字符串比较
来源：http://hz.jinqigufen.top/gtopwwzwbi.html

strcmp(a, b) == 0
来源：http://hz.tianlin.xyz/gtvzrebysd.html

[S07] C：数组遍历求和
来源：http://hz.cheryme.top/gtovpvbhbe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hammf.cn/gtjdxijmpe.html

[S08] C：动态内存分配与释放
来源：http://hz.shuidangran.top/gtjgkzdszn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cdnleiting.top/gtxirizxem.html

[S09] C：结构体定义与初始化
来源：http://hz.yonumen.top/gtkyuhfcal.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hongshengwenyu.top/gtldplzqta.html

[S10] C：指针与解引用
来源：http://hz.tanke756.top/gtaudwcxlb.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gtrwhuqarf.html

[S11] C：逐行读文件
来源：http://hz.yueranfly.top/gtlasheksp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zycfv.cn/gthyesibzu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258.top/gtzefgslbp.html

fclose(f);
来源：http://hz.yvedp.cn/gtcieyfekw.html

[S12] C：写文件
来源：http://hz.xinyue.icu/gtjqgeprcz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guowangkeji.top/gtrtxzwght.html

[S13] C：宏定义
来源：http://hz.cashguo.top/gtxlpobeyk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.bjfxy.top/gtqaasjrjk.html

[S14] C：枚举
来源：http://hz.feifeiyinyue.top/gtfjoeiuov.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhongyouzk.top/gtbfouxqvh.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gtrznqavox.html

(double) a / b
来源：http://hz.cheryme.top/gthakqwvtg.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gtjqamfqfa.html

x |= (1 << 3);
来源：http://hz.shzxlz.cn/gtplultjqk.html

[S17] C：安全拼接字符串
来源：http://hz.c1oappe.top/gtkidxjcfp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gaohongyu789.top/gtpfqgjkix.html

[S18] C：命令行参数
来源：http://hz.jinqigfzy.top/gtgjxlxjgg.html

int main(int argc, char **argv)
来源：http://hz.zdqjudy.top/gttajijnto.html

[S19] C：快速排序
来源：http://hz.wangdashe.top/gtysylybwa.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtoqdpxjln.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gttmnpfhjj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtbkoutsdl.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gtdiukxfrz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtrtznretc.html

[S22] C：字符串转数字
来源：http://hz.sxryk.cn/gtumcdlgca.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtlonxbylq.html

[S23] C：随机数
来源：http://hz.xuanzx.com/gtorsmlgmq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtkrxxgpcs.html

[S24] C：获取本地时间
来源：http://hz.hnqzz.top/gtneioxelp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yongpay.top/gtgqyateif.html

[S25] C：内存拷贝
来源：http://hz.smart0.xyz/gtllraqocb.html

memcpy(dst, src, n);
来源：http://hz.quarkkingdee.top/gtrgmjylyn.html

[S26] C：内存清零
来源：http://hz.nanxinkj.top/gtovicufkf.html

memset(a, 0, sizeof a);
来源：http://hz.xingfuxueyuan.xyz/gtmgsthxsf.html

[S27] C：定义常量
来源：http://hz.shangyingyoupin.top/gtdldkyaxl.html

const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtihdfxvit.html

[S28] C：静态变量
来源：http://hz.yueranfly.top/gtolvnzuhx.html

static int counter = 0;
来源：http://hz.xuanzx.com/gtlowwypmf.html

[S29] C：变参函数
来源：http://hz.feifeiyinyue.top/gtmeymdpir.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.kuanghao11.cn/gtsrwpzrqe.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gttyqmdwuv.html


<!-- 参考信息 -->