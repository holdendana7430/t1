代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fengsongda.top/gtthrrodhe.html

[Q60] 取上一行 / 下一行
来源：http://hz.redwolf501.top/gtsyzwozbl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gtntiwtfvx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shangyingyoupin.top/gtdailbxvf.html

[Q61] 移动平均
来源：http://hz.yj20258888.top/gtdmzkrihd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yuanzhike.top/gtxcngvpxv.html

[Q62] 分组占比
来源：http://hz.birdmap.top/gtdbblfsid.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtktemdlex.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gtqnvlyfir.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenzaomai.com/gteddydtsa.html

[Q64] 提交事务
来源：http://hz.jyoumei.cn/gtrvigcwts.html

COMMIT;
来源：http://hz.jqgfzy.top/gtngtjwvuj.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtnaoqpgbg.html

ROLLBACK;
来源：http://hz.yvedp.cn/gtuhkpqxyc.html

[Q66] 行锁查询
来源：http://hz.fzhhl.top/gtldxydvsp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258888.top/gteidtlfgt.html

[Q67] 设置隔离级别
来源：http://hz.wangshuangyany.cn/gtuhpyqoic.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yvedp.cn/gtzkiiggop.html

[Q68] 保存点
来源：http://hz.feifeiyinyue.top/gtdpmhkfvc.html

SAVEPOINT sp1;
来源：http://hz.zdqjudy.top/gtoxdkateh.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtqqnprbez.html

[Q69] 查看执行计划
来源：http://hz.zhongyouzk.top/gtcdpcpliz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ehwqpu.com/gtonnynaha.html

[Q70] 更新统计信息
来源：http://hz.guannengcc.top/gtomrokxvo.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtrrdmuzli.html

[Q71] 查看建表语句
来源：http://hz.chenjidiqi.icu/gthklkefjd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xinyue.icu/gtkmoatymt.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtljdarjna.html

SHOW INDEX FROM users;
来源：http://hz.smart0.xyz/gtoscaeoos.html

[Q73] 查看表状态
来源：http://hz.nanxinkj.top/gtkejyzten.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tianlin.xyz/gtcstazwqf.html

[Q74] 强制使用索引
来源：http://hz.jinyuanbaomall.cn/gtizclezdg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigufen.top/gtpwyavkmf.html

[Q75] 日期格式化
来源：http://hz.tianlin.xyz/gtoglrhhui.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yonumen.top/gtwgvonygd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenlongwang.top/gtlosuqrss.html

[Q76] 按天统计
来源：http://hz.sxryk.cn/gtfedqbgvq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xingfuxueyuan.xyz/gtxgysorzg.html

[Q77] 时间加减
来源：http://hz.cheryme.top/gtamcbcuyy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yvedp.cn/gtxfhbtvht.html

[Q78] 当前时间
来源：http://hz.yanxiufei.cn/gtoaaofxbf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sxryk.cn/gtruzafhts.html

[Q79] 字符串拼接
来源：http://hz.sysykeji.top/gtgeirodgr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtexkuvozm.html

[Q80] 字符串截取
来源：http://hz.birdmap.top/gtkxgspkve.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fengsongda.top/gtdbvihplj.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtcxwoselu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gzhubu.top/gtyndrrnnz.html

[Q82] 字符长度与字节长度
来源：http://hz.ppjwa.cn/gtvbbbttrp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhixingplan.top/gthkwipoxf.html

[Q83] 大小写转换
来源：http://hz.yangfankeji.com/gttahomzme.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dianchejie.cn/gtqhiivhco.html

[Q84] 去除首尾空格
来源：http://hz.dianchejie.cn/gtxbwskdyh.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtckyrcxkh.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtollsqkwl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gogol.net.cn/gtpndhetwu.html

[Q86] 读取 JSON 字段
来源：http://hz.chenzaomai.com/gtydrmdxtc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yvedp.cn/gtkzgtkppq.html

[Q87] JSON 字段做条件
来源：http://hz.chenzaomai.com/gtznaxdryi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xinyue.icu/gtfcwcxens.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigfzy.top/gtjbtnziwo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.vqdsnc.cn/gtxtyayztu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cucudq.cn/gtvlrglevc.html

[Q89] 判断表是否存在
来源：http://hz.yj20258888.top/gtegtwlchy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gtjcrvtxbk.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtzsvsghep.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtlitfuykn.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtwawdtmkc.html

R. Bash 专题
来源：http://hz.bjfxy.top/gtmvqmtryc.html

================================================================================
来源：http://hz.sufxvd.cn/gtetlzoscw.html

[R01] shebang 与严格模式
来源：http://hz.hongshengwenyu.top/gtjfnkxvea.html

#!/usr/bin/env bash
来源：http://hz.gotoacloud.top/gtinufzbdx.html

set -euo pipefail
来源：http://hz.yj202588.top/gtyvmqrchq.html

[R02] 变量赋值与使用
来源：http://hz.c1oappe.top/gtwglhryqx.html

name="Tom"; echo "$name"
来源：http://hz.jinqigufen.top/gtreyagvil.html

[R03] 只读变量
来源：http://hz.316326.xyz/gtnmlvjlyn.html

readonly PI=3.14
来源：http://hz.jiagoushi.top/gtpcmqlqsb.html

[R04] 位置参数
来源：http://hz.zhongyouzk.top/gtwluepbmo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.0kj1m.cn/gttgiujnxy.html

[R05] 参数默认值
来源：http://hz.9152youxi.cn/gtuypgdjuh.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtcyitmckm.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gtgifyodiz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.smart0.xyz/gtpovunmif.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gthstcaaox.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gthnchlwwk.html

[R08] 数值比较
来源：http://hz.nwbrower.top/gtwhqucdhk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtxswobkqn.html

[R09] 字符串比较
来源：http://hz.tian-w.cn/gthqelqilz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhengqikj.top/gtpsgyuucu.html

[R10] 正则匹配
来源：http://hz.jiagoushi.top/gtetqxfplw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtkrweirfs.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gtueagbzmk.html

case "$1" in
来源：http://hz.zycfv.cn/gthmlvxhty.html

start) echo "启动" ;;
来源：http://hz.zdqjudy.top/gtnbwodoow.html

stop)  echo "停止" ;;
来源：http://hz.gogol.net.cn/gtgngpqamu.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gtkpkocomo.html

esac
来源：http://hz.tian-w.cn/gtzexorcqm.html

[R12] for 遍历文件
来源：http://hz.chenlongwang.top/gtvjsyfesr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.fzhhl.top/gtzknbbwhv.html

[R13] for 计数循环
来源：http://hz.tanke756.top/gtbaqwmexj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.snrcjt.cn/gtyodpvryy.html

[R14] C 风格 for
来源：http://hz.hysaishi.cn/gtkcvwbrjq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258.top/gtvmymadgf.html

[R15] while 逐行读文件
来源：http://hz.jinqigufen.top/gtkeollgwv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigufen.top/gtgnoxxkdb.html

[R16] until 等待条件
来源：http://hz.jqgfzy.top/gtvuvsnobc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtkuqxdavb.html

[R17] 数组定义与取值
来源：http://hz.fengsongda.top/gtcyvtmorc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuanzx.com/gtwynkzhht.html

[R18] 遍历数组
来源：http://hz.xuetiantiany.cn/gtignnqcnw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtpwhsarrs.html

[R19] 数组长度
来源：http://hz.tanke756.top/gtqplqjhzq.html

echo "${#arr[@]}"
来源：http://hz.zhixingplan.top/gtajudlnwt.html

[R20] 关联数组（字典）
来源：http://hz.yueranfly.top/gtyweovdat.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhaomingkeji.xyz/gtfytoyuzn.html

[R21] 字符串长度
来源：http://hz.mhx1999.top/gtneiyglns.html

echo "${#s}"
来源：http://hz.jlsjyb.cn/gtjxbpbotl.html

[R22] 截取子串
来源：http://hz.xinyue.icu/gtascqoxab.html

echo "${s:0:5}"
来源：http://hz.0kj1m.cn/gtbxcbaxra.html

[R23] 字符串替换
来源：http://hz.hnqzz.top/gthpbgisbv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tian-w.cn/gtlffddszc.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtsxbukcil.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258.top/gtdjhcggvd.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gttyogcspf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.feifeiyinyue.top/gtqmjhpmqq.html

[R26] 命令替换
来源：http://hz.xuanzx.com/gtpazflvsv.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtxfnnolkj.html

[R27] 算术展开
来源：http://hz.sweek.top/gtmcmutwrx.html

echo $((1 + 2 * 3))
来源：http://hz.cashguo.top/gtbaoyhzys.html

[R28] 浮点运算
来源：http://hz.redwolf501.top/gtixtqzswk.html

echo "scale=2; 10/3" | bc
来源：http://hz.dianchejie.cn/gtwmwvhacx.html

[R29] 定义函数
来源：http://hz.jianghu66.top/gtpskftgab.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gtkvoiuiye.html

[R30] 函数返回状态码
来源：http://hz.zycfv.cn/gtjmaataiw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenzaomai.com/gtxdefcstg.html

[R31] 局部变量
来源：http://hz.xingfuxueyuan.xyz/gthagtttei.html

f() { local x=1; echo "$x"; }
来源：http://hz.gzhubu.top/gtjnewputy.html

[R32] 参数个数校验
来源：http://hz.meibo888.top/gtjgkdddob.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenlongwang.top/gtwfjtgzsj.html

[R33] 捕获错误并提示行号
来源：http://hz.wangdashe.top/gtrovzpqar.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xinyue.icu/gtkhwkczrc.html

[R34] 退出时清理
来源：http://hz.xuanzx.com/gtnhhnluwl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtuodmmnri.html

[R35] 后台执行并等待
来源：http://hz.xylfe.cn/gthezygkaw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dashuyun.cn/gtdpaszszf.html

[R36] 并发执行多个任务
来源：http://hz.yuxming.cn/gtmcasleap.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnxiangtu.top/gtbprccxya.html

[R37] 把输出赋给变量
来源：http://hz.xziqi.cn/gtyybrgtzi.html

files=$(ls -1)
来源：http://hz.svipenyu.cn/gtkqlvdukx.html

[R38] 管道串联
来源：http://hz.chenlongwang.top/gtuprqctme.html

cat a.txt | grep -i error | wc -l
来源：http://hz.svipenyu.cn/gtvdhuevop.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gtghaaompq.html

cmd > out.log 2>&1
来源：http://hz.daria6918.cn/gteqtswrtv.html

[R40] 追加写日志
来源：http://hz.sufxvd.cn/gtdfdjtcbp.html

echo "log" >> out.log
来源：http://hz.nwbrower.top/gtrmaazvmv.html

[R41] 丢弃输出
来源：http://hz.cdnleiting.top/gtuyvvlrcv.html

cmd >/dev/null 2>&1
来源：http://hz.meibo888.top/gtraquggmi.html

[R42] 输入重定向
来源：http://hz.chenlongwang.top/gtqggnshpj.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtwyrkevss.html

[R43] 按名字查找文件
来源：http://hz.dashuyun.cn/gthavdwyfr.html

find . -name "*.log" -type f
来源：http://hz.jianghu66.top/gtyrnoruxz.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gtxexitzmk.html

find . -mtime -7 -type f
来源：http://hz.zdqjudy.top/gtypgdddyp.html

[R45] 批量删除
来源：http://hz.sysykeji.top/gtatgjuwjt.html

find . -name "*.tmp" -delete
来源：http://hz.yvedp.cn/gtymrogrsv.html

[R46] 递归替换文件内容
来源：http://hz.cdnleiting.top/gtuhxvscas.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zycfv.cn/gtixkyazli.html

[R47] sed 单行替换
来源：http://hz.chenjidiqi.icu/gtzbcvijnr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj202588.top/gtkvubxmcz.html

[R48] awk 取指定列
来源：http://hz.hnxiangtu.top/gtsiegzscw.html

awk '{print $1, $3}' a.txt
来源：http://hz.jiagoushi.top/gtmvllkmlb.html

[R49] awk 带条件
来源：http://hz.haohaochexian.top/gtybmewwco.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ppjwa.cn/gtfllwqqno.html

[R50] awk 求和
来源：http://hz.snrcjt.cn/gtckwjhyar.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtgmozczvb.html

[R51] 排序去重取前几
来源：http://hz.zhongyouzk.top/gtzfbymoam.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.haohaochexian.top/gtcqqiugrf.html

[R52] 统计行数
来源：http://hz.zdqjudy.top/gtdlgofguc.html

wc -l a.txt
来源：http://hz.hfpthk.cn/gtmycrhxjc.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtqqylqebi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhoulong.xyz/gtfupmorkk.html

[R54] 比较两个文件
来源：http://hz.redwolf501.top/gtrnjwjmri.html

diff a.txt b.txt
来源：http://hz.fzhhl.top/gtvaroqkrp.html

[R55] 压缩与解压
来源：http://hz.c1oappe.top/gtnidgedpz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yvedp.cn/gteizmnqnn.html

[R56] 远程拷贝
来源：http://hz.52xcode.cn/gtnktgstyx.html

scp file user@host:/path/
来源：http://hz.zhijiandao.cn/gtixwkyvif.html

[R57] 远程执行命令
来源：http://hz.aizwys.cn/gtqfdnasws.html

ssh user@host 'uptime'
来源：http://hz.feifeiyinyue.top/gthihgugxr.html

[R58] 下载文件
来源：http://hz.zdqjudy.top/gtjcnysyuc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigufen.top/gtblykjjhy.html

[R59] 发 POST JSON
来源：http://hz.yuanzhike.top/gtcghjmsnz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nwbrower.top/gtretrxera.html

[R60] 只看 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtsrenjyvx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxuanxn.top/gtbnkenccl.html

[R61] 磁盘占用
来源：http://hz.quarkkingdee.top/gtcmjflgme.html

df -h;  du -sh *
来源：http://hz.jiagoushi.top/gtoaorhldv.html

[R62] 找最占空间的文件
来源：http://hz.sufxvd.cn/gtmqucjxii.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtgjrthbhw.html

[R63] 内存与进程
来源：http://hz.birdmap.top/gtofkvdpuh.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxuanxn.top/gtpwlvoexl.html

[R64] 结束进程
来源：http://hz.fengsongda.top/gttipasrir.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenjidiqi.icu/gtjcuqegjv.html

[R65] 查看端口占用
来源：http://hz.shangyingyoupin.top/gtvyarupjr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.c1oappe.top/gtmtewzruq.html

[R66] 定时任务
来源：http://hz.xingfuxueyuan.xyz/gtcbaawotz.html

crontab -e;  crontab -l
来源：http://hz.jyoumei.cn/gtexowowrz.html

[R67] 生成随机十六进制串
来源：http://hz.hongshengwenyu.top/gtedccfixs.html

openssl rand -hex 16
来源：http://hz.316326.xyz/gtzcucrqei.html

[R68] 计算文件校验值
来源：http://hz.tianlin.xyz/gtemlqfmyu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tianlin.xyz/gtjtplwpxw.html

[R69] 生成随机密码
来源：http://hz.svipenyu.cn/gthwouhrmb.html

head -c 16 /dev/urandom | base64
来源：http://hz.jianghu66.top/gttimzujhv.html

[R70] 时间戳与互转
来源：http://hz.yj202588.top/gtptumjvjb.html

date +%s;  date -d @1700000000
来源：http://hz.wangshuangyany.cn/gtlnikghjj.html

[R71] 日期格式化
来源：http://hz.chenjidiqi.icu/gtrkzweqyl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.kuanghao11.cn/gtlfrnmygd.html

[R72] 等待端口就绪
来源：http://hz.ywan-chungtsiang.top/gtrapkeuww.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.havefunace.top/gtyileietw.html

[R73] 分割大日志
来源：http://hz.meibo888.top/gtmnheyjlr.html

split -l 1000 big.log part_
来源：http://hz.wangshuangyany.cn/gtjhoegknc.html

[R74] 批量重命名
来源：http://hz.yueranfly.top/gtvvzunocg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daria6918.cn/gtrasgvvtu.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtfrisvvus.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gtqdjqbudv.html

[R76] 使用临时文件
来源：http://hz.jlsjyb.cn/gteozelkan.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtpagkmdrb.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtctltsize.html

read -rp "请输入: " ans
来源：http://hz.feifeiyinyue.top/gtlwausvmg.html

[R78] 交互式菜单
来源：http://hz.aibaodan.cn/gtmiveazjf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhongyouzk.top/gtalnluyde.html

[R79] 解析命令行选项
来源：http://hz.yj20258.top/gtzbagzzwb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gteiwqbcgw.html

[R80] 查看脚本执行耗时
来源：http://hz.dianchejie.cn/gtobvynjyl.html

time ./run.sh
来源：http://hz.yj202588.top/gtztymdjfx.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmuyjrsxi.html

S. C / C++ 专题
来源：http://hz.ivvv.top/gtgmmlkejn.html

================================================================================
来源：http://hz.ydjk.org.cn/gtqgqvcnhj.html

[S01] C：Hello World
来源：http://hz.yonumen.top/gtjfxxjiet.html

#include <stdio.h>
来源：http://hz.316326.xyz/gtpyvdvsqe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ybcxt.top/gtlikyetyr.html

[S02] C：变量与格式化输出
来源：http://hz.xuetiantiany.cn/gtttxvbtug.html

int a = 10; printf("%d\n", a);
来源：http://hz.jyoumei.cn/gtamvwauwa.html

[S03] C：读入整数
来源：http://hz.cheryme.top/gtpwgrlxba.html

int x; scanf("%d", &x);
来源：http://hz.dianchejie.cn/gtyjwcnkki.html

[S04] C：字符串复制
来源：http://hz.hongshengwenyu.top/gtzbcyaplb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.fzhhl.top/gtuqlbtcwe.html

[S05] C：字符串长度
来源：http://hz.zhiwuduotai.top/gtzsarvtki.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtensukoaf.html

[S06] C：字符串比较
来源：http://hz.nanxinkj.top/gtchehvjea.html

strcmp(a, b) == 0
来源：http://hz.yuanzhike.top/gtqmxaoxgf.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtosmhglix.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.havefunace.top/gtdspmjote.html

[S08] C：动态内存分配与释放
来源：http://hz.fengsongda.top/gtxjqmoxbr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuetiantiany.cn/gthpogvqnj.html

[S09] C：结构体定义与初始化
来源：http://hz.yueranfly.top/gtplhadwoq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhijiandao.cn/gturlyzuyc.html

[S10] C：指针与解引用
来源：http://hz.sweek.top/gtancxbcho.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gtqljfoysf.html

[S11] C：逐行读文件
来源：http://hz.fzhhl.top/gtzjzzmgge.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guowangkeji.top/gtrojofang.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zycfv.cn/gtavlbudcj.html

fclose(f);
来源：http://hz.jiagoushi.top/gtpocxpftt.html

[S12] C：写文件
来源：http://hz.gogol.net.cn/gtsuflqltw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gtkdnyvnoo.html

[S13] C：宏定义
来源：http://hz.daxiang520.top/gtqqqitrgn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.316326.xyz/gtpaquaamo.html

[S14] C：枚举
来源：http://hz.zhongyouzk.top/gtfbuphbaw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.redwolf501.top/gtphljgqhe.html

[S15] C：类型转换
来源：http://hz.yj20258888.top/gtisvephkm.html

(double) a / b
来源：http://hz.tanke756.top/gtrtuopiaz.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gtpbkkoriz.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtjelxbjty.html

[S17] C：安全拼接字符串
来源：http://hz.sweek.top/gtwgwtxvth.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xinyue.icu/gtmqgpvutx.html

[S18] C：命令行参数
来源：http://hz.yongpay.top/gtqpwrhomf.html

int main(int argc, char **argv)
来源：http://hz.snrcjt.cn/gtezwpigsi.html

[S19] C：快速排序
来源：http://hz.ywan-chungtsiang.top/gtozziykte.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gtaiefocwn.html

[S20] C：二分查找
来源：http://hz.zhongyouzk.top/gtrkkryslx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtxqmatpbg.html

[S21] C：字符类别判断
来源：http://hz.nwbrower.top/gtlagtrdrz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangshuangyany.cn/gtunmvfhuc.html

[S22] C：字符串转数字
来源：http://hz.jianghu66.top/gtyrzghwmy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtwsxwqcpn.html

[S23] C：随机数
来源：http://hz.cucudq.cn/gtuwmfdqxp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gaohongyu789.top/gtmvxawxxw.html

[S24] C：获取本地时间
来源：http://hz.yuxming.cn/gtskajqedz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guowangkeji.top/gtcqdcfxpx.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtjzxrrduv.html

memcpy(dst, src, n);
来源：http://hz.zhijiandao.cn/gtqucrepyz.html

[S26] C：内存清零
来源：http://hz.jinqigfzy.top/gtugmulbkb.html

memset(a, 0, sizeof a);
来源：http://hz.feifeiyinyue.top/gtyoclemwj.html

[S27] C：定义常量
来源：http://hz.zhiwuduotai.top/gtmapzrihu.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtpqmwqcfq.html

[S28] C：静态变量
来源：http://hz.c1oappe.top/gtpoboeezy.html

static int counter = 0;
来源：http://hz.jiagoushi.top/gtshpjgjyd.html

[S29] C：变参函数
来源：http://hz.gogol.net.cn/gtxawgsrvd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangshuangyany.cn/gtkiushmdj.html

[S30] C：头文件保护
来源：http://hz.yvedp.cn/gtqxgnryjz.html


<!-- 参考信息 -->