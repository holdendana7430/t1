代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2aqesdaws.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2sgmjdsyx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gcwwjcxw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sgcuzpqd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2padtaeah.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ltxosgvs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fttjbrqm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jxymwqlb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2prqkmkzq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ghbvvzzj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2svfgrsgv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2esrxbxrs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hiophcla.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2gydnbdzm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ciuuaary.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cwesirpb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qudbzjwa.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gbijrxxu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kswujzmw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dvtqfaff.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vqgaopjg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dvoatqdh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ebejqzor.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ubnxclmi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2utvvjbhs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2uaobdsna.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2elemxhhk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hkzlxzto.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jkqcpptz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dgxvrsnp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2csxbvutx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sbfxvhgi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2tqaeecqh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eunmmrmm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bcsukwrj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urvutnoe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pkmrpizw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wydyihml.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ojecgmrv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rqcorqda.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2clcqzjxv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xknuperk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nxgaqktm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ngdsoxcp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2oanrylue.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bjegqykv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jrftpvot.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wkifplwl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sryeblro.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2sgngogbl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jmknrxei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnsvyywb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lmdpjcgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awcemssu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2czcatzda.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dlstqkbo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xlonrvaa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yhwnfpoo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jpwmerja.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdasoyjj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zjwbqfwn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kijremox.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zdbhfkzj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eowjunmu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2iuhjulop.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ndlsexjt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzcoyklo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgtxffqt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2aoknvvme.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2oxmiwjgr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2oacgdurv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oeprjwam.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2uxhwiopb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2gwdywvsw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2exgxnudl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2sofoueuw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ybjofwpm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vrbcuhfu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2glczmzds.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dhpxfqnd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2pvinrcbn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yapzjmdl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ezjcrnyc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2iaodpbaf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2puaeggmz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yxxxfdhf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cqhufenx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yatcdgvo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2etexgtnn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2sedvtwww.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tockgzdz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kklzetxa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wskijscl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2alfnsuwx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlbaxhme.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uojqfpqu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qzmzlvej.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gymsvnid.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lonnjdpg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2frulvxoq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wqwadulg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xbjqfyiu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqvhampb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xvianvle.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2hyxbmzxs.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dpczsvak.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2porndyqu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fqwhchcf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2myrvvlkd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ienglycs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ynfkroch.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rkpsgexm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ruovnalx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jtnplpzv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2krcnhuul.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ayoymbze.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2whykcfsd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dqsiufav.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gyutamtb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fzqqlkha.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ocdoypwu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2sjlbbsdg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hkfqzrsr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2teploowd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tiaeyibm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2owoggwjp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fyjbhzzj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2uusaupxz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hvfpoovs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lagsjdug.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nccxliun.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mdbvusru.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2irwmcluw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tfbwajnr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fvujleer.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ytxdjswh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fnteeapd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mhllcosi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jigfyjjk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2btdhtqed.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jmqswqhm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2arjqbhat.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tziwdfsd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2smtdngwg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2laluvomt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2pyucqrcz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2urysjsgs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2pimwfyhb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dmptgexq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2cjofdsed.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xofdmvua.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zkesibin.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gpqxmndw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ztkyqfji.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vqalhgix.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2hfjijcni.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vvpeyfcq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2aymmazgm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2alhqfznc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cwjhmqlx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ibtltigr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xjvoyhrl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qsypknuz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ziqeyigt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tzzmevhd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnoupcvy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uotljlei.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jdumdrtw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uequwogj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bjfsujyo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qfrtxriq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hnnjwpct.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kuujicic.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bpzdpayb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2bkmemwcc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ivhslgby.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qpocizdj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2peodkhjz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2slfhgbpy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ydzzkpio.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rvpzuylr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2faxivlev.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ivsmuubv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2exnyoera.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2dhakccag.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fwlxtqfp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2krudndme.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bjkpdoqb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lttbmiok.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nrsljrhx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pksqfaau.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cmwqiesg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2llurndgn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2micznykz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2tlqdiqzc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2opxoeyyc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wytsczha.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2acfddzrf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nthgrwes.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2flegphvg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2djaxgqsd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ifkvllhk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bgrqiwno.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rdubagxe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jwqjgpvf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2tieszqqg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yvocpxxw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vfvkavxf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cgudspwg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2silqkbkw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cfzmyofa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mzozryge.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zreqloqx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xeyvnfdy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2texlfzgx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hdccqzlb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2znfpyiii.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lhtfodzu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gtwqzuvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykopivof.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nfsccrwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwiaggpz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ccfyqrla.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gagejpjd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcxfcfmg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cxixwiuy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2viufckmz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yxitbfwq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2anofkmuw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mffhfogm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bqwrrnig.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2agpvlvdm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmxqrvda.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2saodmwla.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2badisjdk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pwecceiz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2biwbamdl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2norkytbm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2murvjdgf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wbjvranh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cstbnhgj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2odwqszee.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2efesjarf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lchwwsgw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fkmsvyws.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xxlqdshq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jtkdqjwp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2axaffcca.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nxamkfus.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wmodweys.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2aelafdkp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ommsdngv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2fosywcaf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jqnbptsh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2iccrinvv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2itjmwife.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uifmacvn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oimkfgag.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kfvrrzia.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zyyobynp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2eowmczke.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wyyhpwfm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lpbrhawq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ywvaqqzu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yodysyxp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2kjrkqkrp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gspopqsf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ypkonyro.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2sewpiuiq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ozlvtkrd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rdpkyeux.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hzuhipyf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bmoirldq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hebjrnlx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tkscnuzp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vltbpktw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ghcmwmfq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mukbpnka.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vxmzwbjq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hmkebxac.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2lduxllyj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcfnxceg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2laiifcsq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ooljqhsv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mezfhkeg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iuuofhxj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2gczoumum.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vcakuflb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vlazpmkg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dblcgjsi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xagnforx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2teqgbrgn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dcylninf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tohwblpu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2caczlgjx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvlpjvne.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qbehjnep.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vpwpajup.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2sklyihxj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2excuoszv.html


<!-- 参考信息 -->